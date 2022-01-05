# Simple_cv
Simple_CV_test

1. TF.Установка терраформ
2. AWS.Авторизация в AWS. Получшение Данных для авторизации для TF
3. TF. Создание тераформ файла с описанной инфраструктурой. 
4. AWS. Генерация и установка ssh ключей для авторизации на будущие сервера.
5. TF. Разворачивание инфраструктуры в AWS из 2 инстансов EC2 c Ubuntu 20.04 и Security Group для них. Дополнительно заданы ранее установленные ключи для доступа по ssh.
6. AWS.Первый инстанс был настроен как WebServer для разворачивания на нем будущего сайта. 18.157.161.194 - maydannikov.link
7. AWS.Второй инстанс был настроен как сервер для Jenkins для дальнейшего выполнения на нем небоходимых работ. 18.195.214.70:8888 - http://jenkins.maydannikov.link:8888/
8. HTML/CSS. Был создан не сложный сайт-резюме для дальнейшего использования.
9. Jenkins. На сервер была выполнена первичная настройка с установкой рекомендуемых плагинов.
10. Github. Создан репозиторий и ранее созданый сайт-резюме помещен в него.
11. Jenkins. Создан проект который получает получает новую версию сайта-резюме из репозитория GitHub по ссылке git@github.com:Emaydannikov/Simple_cv.git/
12. Jenkins. Созданы и добавлены ssh ключи для авторизации Jenkins на Github.
13. Jenkins. Настроен тригер для начала сброки из репозитория GitHub - GitHub WebHook.
14. Jenkins. Установлен плагин для валидации html страницы после получения её с GitHub.
15. Jenkins. Добавлен небольшой bash скрипт который проверяет наличие определенных слов в html файле.
16. Jenkins. Настроена авторизация по ssh на ранее подготовленный веб сервер AWS 
17. Jenkins. Добавлена команда перезапуска apache после обновления контента на веб сервере.
18. AWS. В сервисе Route53 было зарегестрировано доменное имя maydannikov.link и установлено ранее используемому веб серверу.
19. AWS. В сервисе Route53 было зарегестрировано доменное имя jenkins.maydannikov.link и установлено ранее используемому серверу Jenkins.