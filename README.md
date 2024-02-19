# Домашнее задание к занятию 10 «Jenkins» - Сергей Ситкарёв

### Подготовка к выполнению

Создать два VM: для jenkins-master и jenkins-agent.

![Задание0](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/01.jpg)

Установить Jenkins при помощи playbook.

Запустить и проверить работоспособность.

Сделать первоначальную настройку.

![Задание0](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/02.jpg)

### Основная часть

Сделать Freestyle Job, который будет запускать molecule test из любого вашего репозитория с ролью.

![Задание1](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/11.jpg)

![Задание1](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/12.jpg)

Сделать Declarative Pipeline Job, который будет запускать molecule test из любого вашего репозитория с ролью.

![Задание1](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/13.jpg)

Перенести Declarative Pipeline в репозиторий в файл Jenkinsfile.

[Jenkinsfile](https://github.com/SSitkarev/ci-04-jenkins/blob/main/Jenkinsfile)

Создать Multibranch Pipeline на запуск Jenkinsfile из репозитория.

![Задание1](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/14.jpg)

Создать Scripted Pipeline, наполнить его скриптом из pipeline.

![Задание1](https://github.com/SSitkarev/ci-04-jenkins/blob/main/img/15.jpg)

Внести необходимые изменения, чтобы Pipeline запускал ansible-playbook без флагов --check --diff, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и запускает прогон с флагами --check --diff.

Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл ScriptedJenkinsfile.

[ScriptedJenkinsfile](https://github.com/SSitkarev/ci-04-jenkins/blob/main/ScriptedJenkinsfile)

Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.