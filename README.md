# dynamoDB

----
Setup local para utilizar o client por linha de comando:

- Fazer download do client:

[Using the AWS CLI - Amazon DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Tools.CLI.html)


# Configuração das credenciais na máquina local:

 

Criar a configuração via linha de comando ou através dos arquivos de propriedades:

- Linha de comando:
```
$ aws configure --profile dev 
```

```
AWS Access Key ID [None]: AKIAI44QH8DHBEXAMPLE 
AWS Secret Access Key [None]: XXXXXXXX
Default region name [None]: us-east-1 
Default output format [None]: json
``` 

- Propriedades:

Configure um perfil default e demais perfis (dev, hom) conforme abaixo: 
```
~/.aws/credentials
```
```
[default]
aws_access_key_id=AKIAIOSFODNN7EXAMPLE
aws_secret_access_key=XXXXXXXX

[dev]
aws_access_key_id=AKIAI44QH8DHBEXAMPLE
aws_secret_access_key=XXXXXXXX
```
```
~/.aws/config
```
```
[default]
region=us-west-2
output=json

[profile dev]
region=us-east-1
output=text
```

 

Para listar profiles:
```
$ aws configure list-profiles default test
```
