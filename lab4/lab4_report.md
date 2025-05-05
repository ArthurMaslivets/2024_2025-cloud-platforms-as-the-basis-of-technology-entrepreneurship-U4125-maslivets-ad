# 2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad
<b>University:</b> [ITMO University](https://itmo.ru/ru/) <br>
<b>Faculty:</b> [FTMI](https://ftmi.itmo.ru) <br>
<b>Course:</b> [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) <br>
<b>Year:</b> 2024/2025 <br>
<b>Group:</b> U4125 <br>
<b>Author:</b> Maslivets Arthur Denisovich <br>
<b>Lab:</b> Lab4 <br>
<b>Date of create:</b> 04.05.2025 <br>
<b>Date of finished:</b> 05.05.2025<br>

Всего у сервиса будет 3 состояния. Начальное, тестирование партнерами и продовое решение. 

***Описание сервиса***:

Сервис принимает текстовые отзывы и определяет их тональность. Пользователь отправляет текст, сервис обрабатывает его с помощью предобученной модели машинного обучения и возвращает результат анализа.

**1: Начальное состояние**

**Описание этапа:**
На этом этапе приложение разрабатывается и тестируется внутри команды. Основной упор на быстрое развертывание и минимальные затраты.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/e39e84de8b9f0478797e75213d3b560ff9876602/lab4/11.png)

**Компоненты:**

•	Cloud Run: Размещение API-сервиса, обрабатывающего запросы.

•	Cloud Storage: Хранение предобученной модели 

•	Firestore: Сохранение истории запросов и результатов анализа.

Стоимость за месяц $:
Cloud Run	4.12 $
Firestore	8.82 $
Cloud Storage	9.90 $
Итого	22.84 $

**Порядок действий:**
1.	Пользователь отправляет текстовый запрос на API, размещённый в Cloud Run.
2.	Cloud Run загружает модель из Cloud Storage.
3.	Модель анализирует текст и определяет его тональность.
4.	Результат сохраняется в Firestore.
5.	Ответ возвращается пользователю.
________________________________________
**2: Тестирование партнёрами**

**Описание этапа:**
На этом этапе сервис предоставляется ограниченному числу человек для тестирования. Требуется обеспечить масштабируемость и сбор аналитики.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/e39e84de8b9f0478797e75213d3b560ff9876602/lab4/12.png)

**Компоненты:**

•	Cloud Run: Обработка запросов и взаимодействие с моделью.

•	Vertex AI Model: Централизованное хранение и управление версиями ML модели.

•	Cloud SQL: Хранение информации о пользователях и аналитических данных.

•	Firestore: Сохранение логов.

•	Cloud Monitoring: Отслеживание метрик и ошибок.

Стоимость за месяц, $:
Cloud Run	70.20 $
Firestore	26.89 $
Vertex AI	72.25 $
Cloud Monitoring 51.11 $
Cloud SQL	115.62 $
Cloud load balancing 82.25  $
Итого	418.32 $

**Порядок действий:**
1.	Пользователь отправляет текстовый запрос на API, размещённый в Cloud Run.
2.	Cloud Run загружает модель из Vertex AI и анализирует текст.
3.	Результаты сохраняются в Cloud SQL и Firestore.
4.	Все сервисы отправляют метрики и логи в Cloud Monitoring
5.	Ответ возвращается пользователю.
_______________________________________
**3: Продовое решение**

**Описание этапа:**
Фокус на этом этапе на обслуживание большого числа пользователей.
 ![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/e39e84de8b9f0478797e75213d3b560ff9876602/lab4/13.png)
 
**Компоненты:**
•	GKE (Google Kubernetes Engine): Размещение и управление контейнерами приложения

•	Vertex AI Model: Централизованное хранение и управление версиями ML модели.

•	Cloud SQL: Хранение информации о пользователях и аналитических данных.

•	Firestore: Сохранение логов.

•	Cloud Monitoring: Отслеживание метрик и ошибок.

GKE	1215.00 $
Firestore	26.89 $
Vertex AI	72.25 $
Cloud Monitoring 51.11 $
Cloud SQL	115.62 $
Cloud load balancing 557.24 $
Итого	2038.11 $

**Порядок действий:**
1.	Пользователь отправляет текстовый запрос на API, размещённый в Cloud Run.
2.	GKE загружает модель из Vertex AI и анализирует текст.
3.	Результаты сохраняются в Cloud SQL и Firestore.
4.	Все сервисы отправляют метрики и логи в Cloud Monitoring
5.	Ответ возвращается пользователю.
