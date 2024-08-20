<u>#**План автоматизации тестирования сценария возможности записи на обучение на курс "Инженер по тестированию"**</u>
##**Перечень автоматизируемых сценариев**
###**Сценарии навигации к странице записи:**

**Сценарий 1: Переход через меню каталога курсов**
-  Открыть страницу сайта Нетологии.
-  Кликнуть на кнопку меню «Каталог курсов».
-  Кликнуть на блок курсов «Программирование».
-  Пролистать страницу до формы «Инженер по тестированию».
-  Кликнуть на курс «Инженер по тестированию».
*Ожидаемый результат:* Открыта страница записи на курс "Инженер по тестированию".

**Сценарий 2: Переход через поисковую строку в каталоге курсов**
-  Открыть страницу сайта Нетологии.
-  Кликнуть на кнопку меню «Каталог курсов».
-  Кликнуть  на поисковую строку "Какой курс Вам нужен?"
-  Ввести в поисковую строку "Инженер по тестированию", нажать Enter
-  Кликнуть на курс «Инженер по тестированию».
*Ожидаемый результат:* Открыта страница записи на курс "Инженер по тестированию".

**Сценарий 3: Переход через блок "Направления обучения"**
-  Открыть страницу сайта Нетологии.
-  Пролистать страницу до блока "Направления обучения"
-  Кликнуть на кнопку "Полный каталог"
-  Пролистать страницу до формы «Инженер по тестированию».
-  Кликнуть на курс «Инженер по тестированию».
*Ожидаемый результат:* Открыта страница записи на курс "Инженер по тестированию".

**Сценарий 4: Проверка функционала выбора курса**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Проверить, что выбранный курс корректно отображается.
*Ожидаемый результат:* Открыта страница записи на курс "Инженер по тестированию".

###**Заполнение и отправка формы записи:**
**Сценарий 1: Успешная запись с валидными данными**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Кликнуть на кнопку «Записаться».
-  Заполнить поля валидными данными:
                          -   Имя (имя на кириллице, например: Александр);
                          -   Номер телефона (11 цифр, например: 79222111018).
-  Кликнуть кнопку "Записаться".
*Ожидаемый результат:* Отображается сообщение об успешной записи и о том, что в ближайшее время с вами свяжутся для оформления на курс.

**Сценарий 2: Ввод невалидного номера телефона, состоящего из 1 цифры**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить поле имя валидным значением.
-  Ввести невалидный номер телефона:
                        -  состоящий из 1 цифры (например, 7).
-  Кликнуть на кнопку "Записаться".
*Ожидаемый результат:* Отображается сообщение об ошибке.

**Сценарий 3: Ввод невалидного номера телефона, состоящего из 10 цифр**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить поле имя валидным значением.
-  Ввести невалидный номер телефона:
-  состоящий из 10 цифр (например, 7922211101).
-  Кликнуть на кнопку "Записаться".
*Ожидаемый результат:* Отображается сообщение об ошибке.

**Сценарий 4: Попытка ввода невалидного номера телефона, состоящего из 12 цифр**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить поле имя валидным значением.
-  Ввести невалидный номер телефона:
-  состоящий из 12 цифр (например, 792221110188).
*Ожидаемый результат:* Отображается сообщение об ошибке.

**Сценарий 5: Попытка ввода невалидного номера телефона, состоящего из нулей**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить поле имя валидным значением.
-  Ввести невалидный номер телефона:
-  состоящий из 10 нулей (например, 70000000000).
*Ожидаемый результат:* Отображается сообщение об ошибке.

**Сценарий 6: Проверка корректности отправки данных на сервер**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить все поля валидными данными.
-  Кликнуть на кнопку "Записаться".
*Ожидаемый результат:* Данные корректно отправлены на сервер и обработаны.

**Сценарий 7: Попытка отправки формы с пустым полем "Имя"**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Оставить поле "Имя" пустым.
-  Заполнить поле "Телефон" валидным значением.
-  Кликнуть на кнопку "Записаться".
*Ожидаемый результат:* Отображается сообщение об ошибке.

**Сценарий 8: Попытка отправки формы с пустым полем "Телефон"**
-  Открыть страницу записи на курс «Инженер по тестированию».
-  Заполнить поле "Имя" валидным значением.
-  Оставить поле "Телефон" пустым.
-  Кликнуть на кнопку "Записаться".
*Ожидаемый результат:* Отображается сообщение об ошибке.


##**Перечень используемых инструментов с обоснованием выбора:**

1.	**Java JDK corretto-11:**
-  Самый востребованный язык для автоматизации, гибкий, универсальный, простой.  Имеет большой набор утилит для решения разных задач и надежный код.
1.	**Gradle:**
-  Инструмент для управления зависимостями и сборки проекта.
1.	**Selenide:**
-  Простота в использовании для тестирования веб-приложений.
-  Стабильность и надежность в работе с динамическими элементами страницы.
1.	**WebDriver:**
-  Стандартный инструмент для управления браузерами, совместимый с Selenide.
1.	**JUnit:**
-  Мощный фреймворк для написания и организации тестов.
-  Поддержка аннотаций, параметризации и гибкой конфигурации тестов.
1.	**Allure:**
-  Средство для генерации наглядных и подробных отчетов о тестировании.
-  Поддержка интеграции с JUnit.
1.	**CI (GitHub Actions):**
-  Автоматизация процессов CI напрямую в репозитории GitHub.
-  Инструмент обнаружения и исправления ошибок на ранних стадиях разработки.


##**Перечень необходимых разрешений, данных и доступов:**
1.	Разрешение на автоматизированное тестирование
2.	Доступ к тестовому серверу сайта.
3.	Требования к входным данным.
4.	Входные данные.
5.	Доступ к  тестовым учетным записям.
6.	 Доступ к API
7.	Документация к API

##**Перечень и описание возможных рисков при автоматизации:**
**1. Отсутствие подключения к интернету:**
-  Отсутствие подключения к интернету может приостановить процесс и привести к увеличению сроков тестирования.
**2. Проблемы с доступом:**	
-  Недоступность тестового сервера может приостановить процесс тестирования.
**3. Изменения в структуре сайта:**
-  Обновления и изменения в верстке страниц могут приводить к поломке тестов.
**4.  Некорректные  данные:**
-  Некорректные тестовые данные могут привести к ошибкам в тестах.
**5.  Сбой в системе:**
-  Сбой в системе может приостановить работу на неопределенный срок, полностью изменив график выполнения запланированного тестирования
**6. Планирование при проектировании селекторов для поиска элементов:**
-  Проектирование селекторов может оказаться более длительным процессом из-за специфичности каждого сайта.


##**Перечень необходимых специалистов для автоматизации**
1.	**Инженер по автоматизированному тестированию:**
-  Разработка тестовых сценариев 
-  Создание автоматизированных тестов.
-  Настройка интеграции c GitHub Actions.
-  Создание отчетности по результатам проведенных тестов.
-  Создание баг-репортов.
##**Интервальная оценка с учётом рисков в часах**
1.	**Исследование и анализ (8-10 часов):**
-  Анализ структуры сайта и способов перехода к странице профессии.
1.	**Разработка тестов для перехода к странице профессии (12-18 часов):**
-  Написание и настройка тестов для различных путей перехода.
1.	**Разработка тестов для перехода к форме записи (6-10 часов):**
-  Написание тестов для пролистывания страницы и нажатия кнопки «Записаться».
1.	**Разработка тестов для заполнения и отправки формы (18-24 часа):**
-  Написание тестов для различных сценариев заполнения и отправки формы.
1.	**Настройка CI (GitHub Actions) (2-3 часа):**
-  Интеграция проекта с GitHub Actions.
1.	**Настройка Allure и генерация отчетов (6-8 часов):**
-  Интеграция Allure и настройка генерации отчетов.
1.	**Тестирование и отладка (16-24 часа):**
-  Тестирование автоматизированных сценариев, выявление и исправление дефектов.
**Итого: 70-100 часов**
