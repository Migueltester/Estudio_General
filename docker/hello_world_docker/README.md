# Practica de docker para realizar un hello world
--- 
## 1. Verificar credenciales
Es este proceso verificamos las credenciales de aws en nuestra consola
a traves del comando 
```sh
aws sts get-caller-identity
```
Tambien podemos verifiacar con
```sh
aws s3 ls --profile <profile>
```

## 2. Creamos una carpeta y clonamos el repositorio con el docker hello world
Este git es un cloudformation, corriendo en un .py que realiza el script de creacion del stack, puedes analizar mas a fondo el repositorio viendolo
https://gitlab.com/-/snippets/4823712
```sh
git clone git@gitlab.com:snippets/4823712.git
```

## 3. abrir enviroment venv
Aqui hay varias maneras de hacerlo, una vez estamos en la carpeta
podemos abrirlo en visual estudio code, ahi ponermos >activar enviroment, luego ahi  seleccionamos los requerimientos, el checkbox y listo comienza a descargar
tambien por dodigo seria
- 1. activar enviroment
```sh
python -m venv venv
```
- 2. entrar en el enviroment
```sh
 source venv/Scripts/activate
```
- 3. Instalamos los requerimientos
```sh
pip install -r requirements.txt
```

## 4. Ya cuando esta el enviroment instalado y todo listo, ya podemos correr el generate.py
Aqui ya lo corres desde el mismo visual estudio code, en el archivo .py editar el perfil 

## 5. iniciamos la instancia en la consola a traves de ssh
```sh
ssh -1 <archivo-llave.pem> <ec2-user@<ip>
```

## 6. Ya iniciado la consola de la ec2 instalamos docker 
```sh
sdo yum install docker -y
```

## 7. ya iniciamos el lab de docker que sera enviado...

```sh
sdo yum install docker -y
sudo systemctl docker
sudo docker hello world
```

```sh
docker run -d -p 80:80 nginx
```

## Practica

1. intenta hacer un volumen persistente de docker del postgress con la info del lab de redes
2. 
