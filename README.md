
`# Local .terraform directories
**/.terraform/*`

Будут проигнорированы файлы с расширением terraform в каталогах различной степени вложенности

`# .tfstate files
*.tfstate
*.tfstate.*`

Будут игнорироваться файлы указаным расширением

`# Crash log files
crash.log
crash.*.log`

исключает файл с указанным названием 

`# Exclude all .tfvars files, which are likely to contain sensitive data, such as
 password, private keys, and other secrets. These should not be part of version 
 control as they are data points which are potentially sensitive and subject 
 to change depending on the environment.
*.tfvars
*.tfvars.json`

Исключит все файлы с расширением .tfvars и  *.tfvars.json

`# Ignore override files as they are usually used to override resources locally and so
 are not checked in
override.tf
override.tf.json
*_override.tf
*_override.tf.json`

Исключаетфайлы с названием и расширением  override.tf.json  и override.tf и а так же файлы которые содержат это название 

`# Include override files you do wish to add to version control using negated pattern
!example_override.tf `

указан пример названия файла содержащего в себе override.tf который не будет индексироваться гитом 

`# Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
 example: *tfplan* `
исключает файлы содержащие в себе tfplan  для использования указанной команды  

`# Ignore CLI configuration files
.terraformrc
terraform.rc `

исключает файлы .terraformrc terraform.rc 
