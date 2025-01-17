# -Zabbix-2-
«Система мониторинга Zabbix. Часть 2» Васяева Ирина
# Задание 1
В данном задании был создан шаблон для мониторинга загрузки CPU и RAM хоста в Zabbix.
## Процесс создания шаблона:
1. Создан новый шаблон с названием `Template_CPU_RAM_Monitoring`. <br/>
2. Добавлен элемент данных для мониторинга загрузки CPU: <br/>
   - Название: Загрузка CPU (в %) <br/>
   - Ключ: `system.cpu.util` <br/>
3. Добавлен элемент данных для мониторинга загрузки RAM: <br/>
   - Название: Загрузка RAM (в %) <br/>
   - Ключ: `vm.memory.size[pused]` <br/>
# Задание 2-3: Установка и настройка Zabbix
### Цель
Добавить два хоста в систему мониторинга Zabbix и настроить Zabbix Agent.
### Хосты
- **vasyaevaia-1** <br/>
- **vasyaevaia-2** <br/>
### Процесс выполнения
В ходе выполнения задания была произведена привязка созданного шаблона к двум хостам (`vasyaevaia-1` и `vasyaevaia-2`) в Zabbix, а также был привязан шаблон **Linux by Zabbix Agent**. <br/>
1. **Установка Zabbix Agent на виртуальные машины:** <br/>
   - Использованы команды для установки в зависимости от ОС. <br/>
2. **Настройка Zabbix Agent:** <br/>
   - Указан IP-адрес Zabbix Server в конфигурационном файле агента. <br/>
   - Запущен сервис Zabbix Agent. <br/>
3. **Добавление хостов в Zabbix:** <br/>
   - Хосты были добавлены с соответствующими именами и интерфейсами. <br/>
   - Прикреплен шаблон `Linux by Zabbix agent`. <br/>
4. **Проверка получения данных:** <br/>
   - В разделе **Latest Data** подтверждено поступление данных от добавленных хостов. <br/>
# Задание 4: Кастомный Дашборд в Zabbix
## Процесс выполнения
В ходе выполнения задания был создан кастомный дашборд в Zabbix с несколькими графиками. Дашборд включает в себя метрики нагрузки ЦП, использования памяти и сетевого трафика. <br/>
### Скриншот дашборда
![image](https://github.com/user-attachments/assets/6d99734a-6954-4b88-80d5-6d71f69fab8f)
