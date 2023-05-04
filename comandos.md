Para subir o deployment com a especificação que você mencionou, você pode executar os seguintes comandos:

Aplicar o arquivo YAML:

kubectl apply -f html-deployment.yml


Expor o deployment como um serviço do tipo LoadBalancer:

kubectl expose deployment app-html --type=LoadBalancer --name=app-html --port=80


O primeiro comando aplica a especificação do deployment definida no arquivo YAML html-deployment.yml.

O segundo comando expõe o deployment como um serviço do tipo LoadBalancer, definindo um nome para o serviço (app-html), a porta do serviço (--port=80) e associando-o ao deployment app-html.


kubectl get service    =    para  ver os serviços


para deletar os serviços     =    kubectl delete service app-html



--------------------------------------------------------------------------------------------------------------


Tabela:

Pod = v1
Deployment = apps/v1
Service = v1