# 2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad
<b>University:</b> [ITMO University](https://itmo.ru/ru/) <br>
<b>Faculty:</b> [FTMI](https://ftmi.itmo.ru) <br>
<b>Course:</b> [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) <br>
<b>Year:</b> 2024/2025 <br>
<b>Group:</b> U4125 <br>
<b>Author:</b> Maslivets Arthur Denisovich <br>
<b>Lab:</b> Lab1 <br>
<b>Date of create:</b> 22.04.2025 <br>
<b>Date of finished:</b> 22.04.2025<br>

**Шаг 1.**  
В разделе IAM & Admin на вкладке Service Accounts создан новый сервисный аккаунт.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/436136777-a7dc1a53-ee04-4470-b48d-df4d0e19c2e2.png)
**Шаг 2.**  
При создании задано название сервисного аккаунта в соответствии с требованиями, указанными в лабораторной работе, затем выполнен переход к следующему этапу.
**Шаг 3.**  
Выбрана роль Storage Admin, после чего сервисный аккаунт успешно создан.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/436138040-ebf67007-169c-4860-867e-eefc39e5ee9e.png)
**Шаг 4.**  
Открыт раздел Compute Engine, на вкладке VM instances нажата кнопка Create instance для создания виртуальной машины.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/436138554-3bbcf9ea-5f9b-4e2d-b5ab-74f14a41ce19.png)
**Шаг 5.**  
Настроены параметры виртуальной машины согласно заданию.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/436140876-9f4a0b9d-18b5-424f-b9d7-899f8d571be4.png)
**Шаг 6.**  
Выполнено подключение к созданной виртуальной машине через SSH.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/Screenshot_3.png)
**Шаг 7.**  
В окне подключения выполнены команды для создания новой папки и копирования в неё необходимых файлов. После выполнения операций SSH-сессия завершена.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/Screenshot_5.png)
**Шаг 8.**  
В разделе IAM & Admin на вкладке Service Accounts для созданного сервисного аккаунта добавлена роль Compute Viewer.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/9faa882802c915cd5264df4c0a6dd822632f5237/lab1/Screenshot_1.png)
**Шаг 9.**  
Повторно выполнено подключение к виртуальной машине через SSH (пробуем то же, что и в шаге 7, но в новой рол). При попытке переноса данных получена ошибка, свидетельствующая о недостаточности прав доступа.
![screenshot](https://github.com/ArthurMaslivets/2024_2025-cloud-platforms-as-the-basis-of-technology-entrepreneurship-U4125-maslivets-ad/blob/5c691eff62bc78bdd82b183968654a6c03d5ec0f/lab1/Screenshot_2.png)
**Шаг 10.**  
Виртуальная машина и сервисный аккаунт удалены.
