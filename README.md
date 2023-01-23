# AWS Serverless Upload Image

Una aplicación sin servidor simple para subir imágenes a Amazon S3 utilizando AWS Lambda y API Gateway.

## Características
- Subir imágenes a S3 utilizando una API RESTful
- Redimensionar automáticamente las imágenes a un tamaño especificado
- Almacenar de manera segura las imágenes con las funciones de seguridad incorporadas de S3

## Comenzando
1. Clone el repositorio: `git clone https://github.com/wilmarcabezas/aws-serverless-upload-image.git`
2. Instale las dependencias necesarias: `npm install`
3. Cree un cubo S3 y actualice la variable `s3Bucket` en `handler.js` con el nombre de su cubo
4. Despliegue la aplicación utilizando el [AWS CLI](https://aws.amazon.com/cli/) o [AWS SAM](https://aws.amazon.com/serverless/sam/)
5. Pruebe la aplicación enviando una solicitud `POST` al punto final de API Gateway con un archivo de imagen como la carga útil

## Configuración
Puede configurar el tamaño de las imágenes actualizando las variables `MAX_WIDTH` y `MAX_HEIGHT` en `handler.js`.

## :warning: Seguridad
Asegúrese de configurar la configuración de seguridad apropiada para su cubo S3 para proteger sus imágenes de acceso no autorizado.

## :books: Recursos
- [Amazon S3](https://aws.amazon.com/s3/)
- [AWS Lambda](https://aws.amazon.com/lambda/)
- [AWS API Gateway](https://aws.amazon.com/api-gateway/)
- [AWS Serverless Application Model (SAM)](https://aws.amazon.com/serverless/sam/)
