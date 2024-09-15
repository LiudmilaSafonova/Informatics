## Отчет по Лабораторной работе 1

Для начала работы я скачала виртуальную машину VMware и дистрибутив Linux Ubuntu. После открыла терминал и выполнила работу.

На фото представлены все вводимые мной команды.
![Screenshot 2024-09-15 184211](https://github.com/user-attachments/assets/3d5f47db-708c-42f4-a1e4-96fb154e4485)


* 1-5 команды, необходимые для установки Ubuntu

* 6 - создание файла script.bash
```bash
touch script.bash
```

* 7 - превая попытка открыть файл в редакторе gedit. В командной строке вывело ответ, что gidit не установлена в моей системе. Были предложены 2 варианта установки gidit, я выбрала первый.
![Screenshot 1](https://github.com/user-attachments/assets/e92aedc5-a56d-42c5-b31c-b7d4fd563883)

* 8 - для установки gedit потребовалось зайти в суперпользователя
![Screenshot 2](https://github.com/user-attachments/assets/e10fe12c-f056-48c9-82c8-c5554f89d8e4)

* 9 - Открыла файл в gedit и написала команду, выводящую фразу "Welcome to ITMO University". 
  ![Screenshot 2024-09-15 172628](https://github.com/user-attachments/assets/e9735a89-057b-4a38-96f1-ef6859777ccf)

* 10 - при запросе командой bash вывело результат
  ![Screenshot 2024-09-15 172734](https://github.com/user-attachments/assets/2ee9b249-c0bd-4df3-bff7-2eb85dc7bac2)

* 11 - далее изменила script.bash, чтобы файл мог выводить неопределенное количество аргументов (частей имени) в виде
```
Welcome, var1 var2 ... varn
```
где varn - последняя часть имени

для этого написала такой код
![Screenshot 2024-09-15 173008](https://github.com/user-attachments/assets/a4b76596-4b4a-4cfe-b276-c406636156bf)

1. т.к. мне были нужны все позиционные параметры (аргументы командной строки), количество которых неизвестно, использовала специальную переменную $@. 
2. использовала цикл for, чтобы перебрать все элементы (в цикле названы var), хранящиеся в $@.

* 12 - 14 проверка вывода
  ![Screenshot 2024-09-15 173356](https://github.com/user-attachments/assets/dbc9263c-9cfd-4423-80ce-97ed7a53d83b)






