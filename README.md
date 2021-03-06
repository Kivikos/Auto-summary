![image](https://user-images.githubusercontent.com/16463676/158784028-957a35eb-9b78-4d57-ab62-8bf9da255e72.png)


# Тестирование возможности записи на обучение профессии "Тестировщик ПО"

# Тест - план

## 1. Перечень автоматизируемых сценариев
  - Заполнение формы для последующей записи на обучение через первую кнопку "Записаться" на странице профессии, расположенную сразу после краткого описания курса
  - Заполнение формы для последующей записи на обучение через вторую кнопку "Записаться" на странице профессии, расположенную в появляющейся дополнительной строке вверху сайта при пролистывании страницы профессии
  - Заполнение формы для последующей записи на обучение через форму записи на обучение и консультацию "Запишитесь или получите консультацию"

*Примечание* - при выполнении тестирования необходимо учесть, что зайти на страницу профессии "Тестировщик ПО" возможно тремя способами: 
1. Нажать на кнопку списка "Каталог курсов" - выбрать вкладку "Программирование" - выбрать профессию "Тестировщик ПО".
2. Пролистать страницу вниз до блока "Направления обучения" - выбрать модуль "Программирование" - выбрать прфоессию "Тестировщик ПО".
3. Выбрать блок "НЕО для начинающих" - выбрать профессию "Тестировщик ПО".

### Ожидаемые результаты выполнения сценариев:

1. В форму вводятся валидное имя и валидный телефон - отсутствие сообщения об ошибке в введенных данных .
2. В форму вводятся валидное имя и невалидный телефон - появление сообщения об ошибке в введенном номере телефона.
3. В форму вводится валидное имя, поле "Телефон" пустое - появление сообщения "Номер телефона не указан".
4. В форму вводится валидный телефон, поле "Имя" пустое - появление сообщения "Имя не указано".
5. В форме остаются пустыми поле "Имя" и поле "Телефон" - появление сообщения "Имя и телефон не указаны".
6. В форму вводится невалидное имя и валидный телефон - появление сообщения "Имя указано неверно".
7. В форму вводится невалидное имя и невалидный телефон - появления сообщения "Имя и телефон указаны неверно".


## 2. Перечень используемых инструментов с обоснованием выбора
- Браузер Google Chrome - для доступа к сайту
- Java 11 - язык программирования
- IntelliJ IDEA - IDE для написания и выполнения тестов
- Maven/Gradle - обеспечение возможности подключения дополнительных инструментов при выполнении тестирования
- JUnit Jupiter- для запуска тестов
- Selenium - для поиска элементов на HTML-странице
- Allure - для генерации расширенных и удобных отчетов о тестировании
- Faker - для генерации рандомных данных

## 3. Перечень необходимых разрешений/данных/доступов
1. Разрешение на проведение автоматизированного тестирования
2. Тестовые данные (от разработчиков или сгенерированные Faker):
- валидное имя, валидный телефон
- валидное имя, невалидный телефон
- невалидное имя, валидный телефон
- невалидное имя, невалидный телефон
- пустое поле "Имя", валидный телефон
- валидное имя, пустое поле "Телефон"
- пустое поле "Имя", пустое поле "Телефон"

## 4. Перечень и описание возможных рисков при автоматизации
### При наличии тестировщика - автоматизатора в штате: 
1. Постоянное отслеживание актуальности автотестов:
- отслеживание актуальности выбранных локаторов;
- отслеживание актуальности структуры сайта;
- отслеживание работоспособности сайта.
3. Выделение дополнительного времени и ресурсов на автоматизацию тест-кейсов.
4. Некорректные автотесты (ничего не проверяют).
### При отсутствии тестировщика - автоматизатора в штате:
1. Дополнительные затраты ресурсов и времени на найм инженера-автоматизатора или на профессиональную переподготовку инженера по ручному тестированию - в любом случае вызывает увеличение стоимости тестирования.
2. см. риски "при наличии тестировщика - автоматизатора в штате"

## 5. Перечень необходимых специалистов для автоматизации
1. Инженер по автоматизированному тестированию

***или***

2. Инженер по ручному тестированию, готовый обучиться на инженера-автоматизатора


## 6. Интервальная оценка с учётом рисков (в часах)
При наличии в штате инженера-автоматизатора: ***56 часов***

При отсутствии в штате инженера-автоматизатора: ***не поддается исчислению, так как зависит от времени найма, обучения и прочего***
