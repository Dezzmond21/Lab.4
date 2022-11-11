# Lab.4
Lab.4

1.Створення SSH ключа

![image](https://user-images.githubusercontent.com/46502035/201242686-c1387fe5-c4bc-4368-a02c-95bf9e6f2b5f.png)

2.Додавання SSH ключа в аккаунт на GitHub

![image](https://user-images.githubusercontent.com/46502035/201244520-4b5260f2-d28e-4941-b01a-ac4aaa5f143f.png)

3.Робота с гілками

![image](https://user-images.githubusercontent.com/46502035/201248637-032c82a5-f8ef-43ac-987f-e4d308e51e03.png)

![image](https://user-images.githubusercontent.com/46502035/201248668-148f23a1-30fd-4af3-acff-1461d846528c.png)

![image](https://user-images.githubusercontent.com/46502035/201248703-01181e33-e77f-45c8-bfd2-fed6e8248041.png)

![image](https://user-images.githubusercontent.com/46502035/201248785-6d896f3b-0269-4b98-abf6-26f652dd40e0.png)

![image](https://user-images.githubusercontent.com/46502035/201248824-86c46e7c-93f1-4e7b-8c32-4f212a996124.png)

![image](https://user-images.githubusercontent.com/46502035/201248851-1f26a263-ef1b-42bb-b643-c1f1c5cc4630.png)


Висновок

В ході лабораторної роботи було розглянуто питання щодо створення
SSH ключа і клонування репозиторію з його допомогою, була реалізована
робота з гілками і вирішення конфлікту злиття гілок.

Контрольні запитання
1. Як створити SSH ключ?

Для створення SSH ключа необхідно виконати такі дії:
– запустити консоль керування Git за допомогою команди git-bash;
– вставити текст, наведений нижче, замінивши адресу електронної
пошти на потрібну і натиснути Enter:
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"


2. Як додавання SSH ключа в аккаунт на GitHub?

Для додавання SSH ключа в аккаунт на GitHub необхідно виконати
такі дії:
– копіювати ключ і прописати його в командному рядку в консолі (копіює в буфер обміну ключ):
clip < ~/.ssh/id_rsa.pub
– зайти на GitHub в розділ Settings;
– в меню SSH and GPG keys натиснути на кнопку New SSH key;
– у полі Title написати назву ключа, а в поле Key вставити скопійований ключ;
– натиснути Add SSH key і підтвердити свій пароль у спливаючому вікні.

5. Як вирішити конфлікт при злитті гілок?

Для того щоб вирішити конфлікт, необхідно прибрати зайві знаки
(<,=,>)і залишити тільки ту частину коду, яка необхідна.

7. Як зберегти зміни у репозиторії після вирішення
конфлікту злиття гілок?

Написати git add . потім git commit -m "що сталося в зміні" а потім написати git push

5. Як у файлі позначається конфлікт при злитті гілок?

Git позначає конфлікт таким чином, що від стрілок <<< до === –
це зміни з першої гілки яку зливали, а от === до стрілки >>> зміни з другої
гілки.
