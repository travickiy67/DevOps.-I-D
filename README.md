# Травицкий Сергей
# Домашнее задание к занятию «Что такое DevOps. СI/СD»

### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` [репозитория c шаблоном решения](https://github.com/netology-code/sys-pattern-homework) к себе в GitHub и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw.
   2. Выполните клонирование этого репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите сверху название занятия, ваши фамилию и имя;
      - в каждом задании добавьте решение в требуемом виде — текст, код, скриншоты, ссылка.
      - для корректного добавления скриншотов используйте [инструкцию «Как вставить скриншот в шаблон с решением»](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md);
      - при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md).
   4. После завершения работы над домашним заданием сделайте коммит `git commit -m "comment"` и отправьте его на GitHub `git push origin`.
   5. Для проверки домашнего задания в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем GitHub.
   6. Любые вопросы по выполнению заданий задавайте в чате учебной группы или в разделе «Вопросы по заданию» в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!

---

### Задание 1

**Что нужно сделать:**

1. Установите себе jenkins по инструкции из лекции или любым другим способом из официальной документации. Использовать Docker в этом задании нежелательно.
2. Установите на машину с jenkins [golang](https://golang.org/doc/install).
3. Используя свой аккаунт на GitHub, сделайте себе форк [репозитория](https://github.com/netology-code/sdvps-materials.git). В этом же репозитории находится [дополнительный материал для выполнения ДЗ](https://github.com/netology-code/sdvps-materials/blob/main/CICD/8.2-hw.md).
3. Создайте в jenkins Freestyle Project, подключите получившийся репозиторий к нему и произведите запуск тестов и сборку проекта ```go test .``` и  ```docker build .```.  

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.  

**Скрин 1.1**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.0.png)  

**Скрин 1.2**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.2.png)  

**Скрин 1.3**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.3.png)  

**Скрин 1.4**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.4.png)  

**Скрин 1.5**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.5.png)  

**На 15 сборке команда push прошла успешно.**  

**Скрин 1.6**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins1.6.png)  

---

### Задание 2

**Что нужно сделать:**

1. Создайте новый проект pipeline.
2. Перепишите сборку из задания 1 на declarative в виде кода.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.  

**Скрин 2.1**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins2.1.png)  

**Скрин 2.2**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins2.2.png)  

**Скрин 2.3**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins2.3.png)  

**Скрин 2.4**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins2.4.png)  

---

### Задание 3

**Что нужно сделать:**

1. Установите на машину Nexus.
1. Создайте raw-hosted репозиторий.
1. Измените pipeline так, чтобы вместо Docker-образа собирался бинарный go-файл. Команду можно скопировать из Dockerfile.
1. Загрузите файл в репозиторий с помощью jenkins.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.  

**Скрин 3.1**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.1.png)  

**Скрин 3.2**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.2.png)  

**Скрин 3.3**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.3.png)  

**Скрин 3.4**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.4.png)  

**Скрин 3.5**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.5.png)  

**Скрин 3.6**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.6.png)  

**Это мои удачные и не удачные попытки сборок.**

**Скрин 3.7**  

![alt text](https://github.com/travickiy67/DevOps.-I-D/blob/main/img/jenkins3.7.png)  
---

