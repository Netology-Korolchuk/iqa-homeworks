
# Домашнее задание к занятию 1.3. Тестирование ПО. Многообразие тестирования
## Задание 1

Рассмотрим кейсы. Какие техники тест дизайна, изученные на уроке, вы бы применили к каждому из кейсов и что именно вы бы стали проверять. Объясните, почему?

Кейсы:

1. Допустим, вы получили задание протестировать новый лендинг* от Альфа-Банка: https://alfabankbumblebee.ru/. 
Делали его срочно к премьере фильма, так что вы его видите в первый раз и к тому же на него почти нет документации. Что и как бы вы стали проверять? 
* Лендинг - это, как правило, одностраничный сайт, который может быть как страницей подписки на что-то бесплатное, так и страницей продажи некого товара или услуги.

2. Вам пришло задание на тестирование нового калькулятора ипотеки. Так как это важный функционал, у нас есть все нужное для тестирования - тестовые юзеры, информация про требования и тестовая среда, где мы можем все проверить до запуска продукта. Ваша задача - проверить весь функционал именно калькулятора: https://alfabank.ru/get-money/mortgage/programs/digital-ab/#calc
С применением каких техник вы стали бы это делать?

3. Представим, что вы уже несколько лет тестируете приложение Альфа-Банка для iOS и вам пришла задача, в которой написано, что разработчики бэкенда переделали систему хранения данных о зарегистрированных пользователях и им важно знать, что ничего не сломалось на фронтенде приложения. Что и по каким методикам вы будете проверять при условии того, что у нас сжатые сроки по тестированию?

Результат задания: номер кейса; название техники, которую вы выбрали; пояснение, почему выбрали именно ее.

## Ответ: 
1. Метод исследовательского тестирования - нет документации, планов, тест-кейсов и прочего. 

2. Метод белого ящика и альфа-тест - у нас есть тестовая среда, тестовые юзеры и вся информация. Вид тестирования модульный - нам нужно протестировать функционал только калькулятора.

3. Метод на основе опыта - мы несколько лет тестируем это приложение. Вид -тестирование сборки.

## Задание 2 

Представим, что мы тестируем форму получения карты банка. В данном случае нам нужно применить знания, полученные на лекции для проверки ввода информации в поле "Имя"

![Image of the game](https://github.com/netology-code/iqa-homeworks/blob/master/1.3/img/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.png)

Что нам известно по спецификации:
Пользователь должен ввести данные, чтобы оформить заявку. Максимальная длина поля 30 символов, минимальная - 1.

Наша задача - проверить максимальное количество вариантов ввода данных, как валидных для системы, так и невалидных. Совет: задумайтесь над проверкой не только позитивных вариантов, но и негативных неописанных в спецификации, так как наша задача - не только проверить соответствие спецификации, но и изучить ситуации, не описанные в ней.

Для получения зачета нужно как минимум 10 вариантов ввода данных в поле имени.

Результат задания: список вариантов ввода имени.

## Ответ: 
1. s - минимальная длина
2.  - пустое значение
3. йx30 - максимальная длина
4. ормормвйгмгннйцгнуепгнйцугнпйгцнупгнймцвгмгнймцвмгмцйвгмгмйцв - больше максимальной длины.
5.   sadsasd - пробелы в начале.
6. ыфвфывфыв   - пробелы в конце.
7. <body> - html теги.
8. Ъ bє{|│Ке - не ASCII символы.
9. ыфыв ыфыв ыфыв - пробелы в середине и повторяющееся значение.
10. Вячеслав - верное валидное значение.
 и др.

Вот здесь я, например, не нашел только 2 значения:
![Image of the game](https://github.com/Netology-Korolchuk/iqa-homeworks/blob/master/1.3.%20%D0%A2%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%9F%D0%9E.%20%D0%9C%D0%BD%D0%BE%D0%B3%D0%BE%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%B8%D0%B5%20%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F/222.jpg)
 -----
 
Задание 1.

Кейс 1: Все верно, применяется исследовательское тестирование. Но необходимо ответить на вопрос: "Что и как бы вы стали проверять?"

Кейс 2: Могу не согласится с тестирование белого ящика, так как нам известны только требования, а не исходных код. Альфа-тестирование - слишком обширное понятие. Любая Ваша деятельность на этапе тестирования нового функционала будет фактически являтся альфа-тестированием. Подумайте, какие техники можно применить, зная требования этого нового функционала, и имея необходимые тестовые данные.

Кейс 3: Верно, на основе опыта работы с приложением специалист знает всего его сильные и слабые стороны. Но одним тестирование сборки здесь не обойтись. Но чтобы вы сделали, зная что поменялось и то как работает приложение? Опишите, пожалуйста.



Задание 2.
Вы нашли отличный портал, на котром можно проверить свои знания!
Но 
"йx30 - максимальная длина" - это не максимальная длина, здесь всего 4 символа.

И личная рекомендация: лучше использовать корректные данные, вместо набора символов и букв, как например: ормормвйгмгннйцгнуепгнйцугнпйгцнупгнймцвгмгнймцвмгмцйвгмгмйцв 

