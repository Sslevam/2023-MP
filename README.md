# 2023-MP
ННГУ, методы программирования, практика по курсу 2023 года

Презентация по курсу (обновляемая): https://docs.google.com/presentation/d/1wmYjy5QDoYECEHi7NAAINPulU9pLsaIi-aLaUppspps/edit?usp=sharing

Для работы необходим python 3.9 и выше. Библиотеки: numpy, pandas, matplotlib, tensorflow, Pillow, scipy.signal. Редактор любой. Из неплохих: IDLE (родной, идёт вместе с установщиком), Visual Studio Code, notepad++, PyCharm, vim (для любителей сначала страдать, потом наслаждаться).

Работа с блокнотами онлайн, с возможностью подключения удалённых мощностей гугла (GPU, TPU): https://colab.research.google.com/

Таблица, где я буду отмечать сданные работы: https://docs.google.com/spreadsheets/d/1ukuncwEtZQ2gwp6FhGD3waF9M96D4eBTSghJeSzotjg/edit?usp=sharing

Сервер в Дискорд, где буду дублировать: https://discord.gg/MzPkCYf4Dh (получить роль в канале "Основной") Мой контакт: nsmorozov@rf.unn.ru

Внутри папки группы создать папку имени себя (фамилия и имя). В своей папке можете делать все что угодно, в чужие не залезать, в корневую тоже. Я буду ориентироваться на файлы, где в названии будет номер лабораторной.

## [1] Работа со структурами данных
	
Исходные данные:

- свои ФИО, число, месяц, год рождения в виде кортежа;
- предметы в школьном аттестате (не меньше 14), как словарь из названия и оценки (можно мокать);
- имена (только) ближайших (до двоюродных включительно) родственников в списке;
- имя, которое вы бы дали своей домашней пушистой киве (строка).

Действия:

1) вывести среднюю оценку в аттестате;
2) вывести уникальные имена среди своих родственников (включая свое);
3) общая длина всех названий предметов;
4) уникальные буквы в названиях предметов;
5) имя вашей домашней пушистой кивы в бинарном виде;
6) отсортированный по алфавиту (в обратном порядке) список родственников;
7) количество дней от вашей даты рождения до текущей даты (должна быть всегда актуальной);
8) FIFO очередь, в которую можно добавлять предметы по вводимому с клавиатуры индексу (до команды остановки), после введения - вывести все;
9) по введеному индексу, поменять имя в отсортированном списке родственников на имя ацтекского правителя (смотреть по списку всех на странице https://en.wikipedia.org/wiki/List_of_rulers_of_Tenochtitlan) под номером, получаемым из вашей даты рождения: number = (day + month**2 + year) % 21 + 1;
10) создать связный список, например, как словарь, где ключ - имя родственника, а значение (ссылка на следующий элемент) - индекс следующего имени по исходному списку, упорядоченному по их (родственников) годам рождения), исходный список при этом должен остаться неизменным;
11) написать функцию-генератор, свой вариант определяется как number = len("ФИО") * len (family_names) % 4:

	0. аликвотной последовательности; 
	1. последовательности Сильвестра; 
	2. числа трибоначчи; 
	3. числа Леонардо. 
