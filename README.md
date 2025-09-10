# Taller de Terraform

Alejandro Amu Garcia – A00395686

## Acceso al azure

<img width="921" height="456" alt="image" src="https://github.com/user-attachments/assets/34895f6c-4afe-4bd4-b0de-039e2fd29301" />

Para empezar se hizo el login al azure mediante cli haciendo uso del comando `az login`, para posteriormente seleccionar la cuenta con la cual se quería trabajar.

Luego se ejecutó el comando `az account show` para ver la información de la cuenta y así obtener datos que nos serán útiles más adelante.

<img width="921" height="490" alt="image" src="https://github.com/user-attachments/assets/b435a62f-c546-49cf-a051-3f0a6dc17f3b" />


Posteriormente dentro de la carpeta del proyecto que se va a desplegar, se ejecutó el comando `terraform init`, con el objetivo de instalar todos los paquetes necesarios para el proyecto dependiendo de los recursos que se hayan definido en el archivo.

En este caso todos los paquetes necesarios ya están instalados.  

<img width="921" height="290" alt="image" src="https://github.com/user-attachments/assets/8c63ee10-ddc1-4fe3-8fdb-968a8690b0a3" />


Posteriormente añadimos el `subscription_id` al provider, el cual obtenemos de la Azure CLI en la línea que se muestra en la siguiente imagen.

<img width="921" height="451" alt="image" src="https://github.com/user-attachments/assets/5cce605d-4abc-4ee1-8de2-223bbc5abd56" />


Posteriormente ejecutamos el comando para asegurarnos de que el archivo esté correctamente escrito, indentado y formateado.  

<img width="921" height="48" alt="image" src="https://github.com/user-attachments/assets/6046022d-64ab-45bb-9d5f-316abb88429a" />


Luego 

<img width="921" height="257" alt="image" src="https://github.com/user-attachments/assets/0146136f-15e2-4f96-99a0-3a006fe079c5" />


ejecutamos el comando `terraform plan` esto con el fin de que se muestren todos los cambios o todos los archivos que se van a subir.  

<img width="921" height="98" alt="image" src="https://github.com/user-attachments/assets/f5276edd-b329-416f-9044-9803c0b4b1a6" />


Validamos con el comando `terraform validate` para asegurarnos de que todo esté correcto.  
<img width="921" height="401" alt="image" src="https://github.com/user-attachments/assets/a8395f82-7064-4cb4-8b17-5d6584c4bedd" />

Finalmente ejecutamos el comando `terraform apply` y vemos como se sube todo el proyecto.

En este caso como todos los pasos se habían hecho previamente y no se hicieron cambios al archivo original, no se añadieron, cambiaron o destruyeron ninguno de los recursos.

<img width="921" height="428" alt="image" src="https://github.com/user-attachments/assets/22643a1f-7f78-4721-8c58-9bdcd95c22b7" />


En el portal de Azure podemos ver cómo fue desplegada la función bajo el nombre: **amumiprimerafuncion**.


<img width="1083" height="152" alt="image" src="https://github.com/user-attachments/assets/0483d341-e96b-4e47-8917-b3e30fd4d0c5" />


Y vemos como en efecto, al ir a la url del despliegue, el codigo funciona correctamente
