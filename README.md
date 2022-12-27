# 7.6_Provider_Aleksandr_Molokov

## Задача 1. 
Давайте потренируемся читать исходный код AWS провайдера, который можно склонировать от сюда: 
[https://github.com/hashicorp/terraform-provider-aws.git](https://github.com/hashicorp/terraform-provider-aws.git).
Просто найдите нужные ресурсы в исходном коде и ответы на вопросы станут понятны.  


1. Найдите, где перечислены все доступные `resource` и `data_source`, приложите ссылку на эти строки в коде на 
гитхабе.   
1. Для создания очереди сообщений SQS используется ресурс `aws_sqs_queue` у которого есть параметр `name`. 
    * С каким другим параметром конфликтует `name`? Приложите строчку кода, в которой это указано.
    * Какая максимальная длина имени? 
    * Какому регулярному выражению должно подчиняться имя? 
    
## ОТВЕТ

1. Найдите, где перечислены все доступные `resource` и `data_source`, приложите ссылку на эти строки в коде на 
гитхабе.

resourse - перечислены в файле provider.go, строки с 943 по 2221, файл расположен в internal\provider\

![1 resource](https://user-images.githubusercontent.com/109212419/209714483-785e0350-abdd-43e9-9076-0cc499ccfc2f.jpg)

![2 resource](https://user-images.githubusercontent.com/109212419/209714496-0c992233-d1c2-4cbd-ad8d-fa27621f49d2.jpg)


data_source - перечислены в файле provider.go, строки с 419 по 941,  файл расположен в internal\provider\

ссылка - 		DataSourcesMap: map[string]*schema.Resource{

![1 data source](https://user-images.githubusercontent.com/109212419/209714752-09419d7f-cb47-49d0-ba37-c0e76e7c7463.jpg)

![2 data source](https://user-images.githubusercontent.com/109212419/209714758-34c2f2e1-1ace-4ac2-9abd-ea8fc64a021f.jpg)



