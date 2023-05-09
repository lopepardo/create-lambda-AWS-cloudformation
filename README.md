# Creando una función lambda con AWS CloudFormation

Este repositorio contiene un ejemplo de como crear una función lambda con AWS CloudFormation.

## Requisitos

- [AWS Account](https://aws.amazon.com/)
- [AWS CLI](https://aws.amazon.com/cli/)

## Funcionalidad

- Crear un stack de CloudFormation con una función lambda y un rol de IAM.
- Actualizar el stack de CloudFormation con una nueva versión de la función lambda.
- Eliminar el stack de CloudFormation.

## Ejecución

´´´bash
aws cloudformation create-stack --stack-name lambda-example-stack --template-body file://LambdaExample.yaml --capabilities CAPABILITY_NAMED_IAM
´´´

´´´bash
aws cloudformation update-stack --stack-name lambda-example-stack --template-body file://LambdaExample.yaml --capabilities CAPABILITY_NAMED_IAM
´´´

´´´bash
aws cloudformation delete-stack --stack-name lambda-example-stack
´´´
