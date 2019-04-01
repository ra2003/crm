Построена на базе платформы [lsFusion](https://github.com/lsfusion/platform).

# Возможности

* Ведение клиентов, организаций, а также контактных лиц по ним.
* Поддержка нескольких собственных компаний.
* Работа с договорами, соглашениями и актами.
* Возможность генерации документов на основе шаблонов (Word) и заготовок.
* Ввод/импорт оплат клиентов и собственных платежей из бухгалтерского контура.
* Контроль рабочего времени сотрудников. Поддержка отпусков, больничных, отгулов. Импорт из Redmine.
* Поддержка разных валют.
* Поддержка расходов по сотрудникам. Расчет прибыли по клиентам.
* Регистрация событий по клиентам.

# Демо

Демо-версия с наполненной тестовой базой данных находится по адресу https://demo.lsfusion.org/crm.

В примере введены пользователи с разными ролями и доступными формами.

Доступные логины :
* admin - Администратор (полный доступ ко всем функциям)
* owner - Учредитель
* manager - Менеджер
* accountant - Бухгалтер
* employee - Сотрудник

Пароли совпадают с логинами.

Изменять роли и их права можно под администроторм на форме Администрирование / Политика безопасности.

# Краткое описание

Основные рабочие формы расположены на вкладке Рабочий стол. Каждая из них предназначена для выполнения определенного процесса(ов).

## Мои задачи

Предназначена для создания задач другим сотрудниками и изменению назначенных текущему пользователю задач. Показываются только задачи не импортированные из внешних систем (например, Redmine)

## Обработка документов

Показывает список всех рабочих документов (договора, соглашения, акты) в системе в единой таблице. Предназначена для работы со входящей и исходящей корреспонденцией. В этой форме можно отмечать даты и способы отправки документов, закрывать обработанные.

## План платежей

Показывает помесячно задолженности (будущие и текущие) в разрезе типов договоров, а также произведенные оплаты.

## Работа с клиентами

Форма предназначена для удобного отображения и редактирования всей информации по одному клиенту. 

## Прибыль по клиентам

Рассчитывает за выбранный интервал доходы, расходы и прибыль в валюте. Доходы рассчитываются как все платежи по курсу на дату оплаты. Расходы рассчитываются исходя из отмеченного времени сотрудников по клиентам исходя из сумм, заданных в форме Расходы по сотрудникам. Также отмеченное время по проектам без клиента (внутренним проектам) может "расписываться" на всех клиентов пропорционально доходам относительно групп договоров.

## Работа с договорами

Показывает список всех активных договоров с возможностью их редактирования и просмотром всей детальной информации, привязанной к договорам.

## Контроль отмеченного времени

Показывает в виде таблицы отмеченное время и отсутствие каждого сотрудника за определенный месяц. Необходима для контроля менеджером правильности заполнения табеля рабочего времени сотрудниками.

## Обработка событий

На этой форме пользователи могут регистрировать события (звонки, переговоры, презентации и т.д.) связанные с определенными клиентами. Также в ней можно отслеживать время необходимости следующего контакта с клиентом, если это было помечено ранее, через отбор Последние по клиенту.

## Табель рабочего времени

Предназначена для отметки сотрудниками времени, затраченного по конкретным клиентам, а также регистрации отпусков, больничных и прочих причин остуствия на рабочем месте. Если осуществляется автоматический импорт из внешней системы отметки времени (например, Redmine), то в форме отображаются также и импортированные отметки времени.

## Контроль задолженности

Отображает список задолженностей по всем договорам клиентов. Идет автоматический расчет суммы оплаты по каждой задолженности с учетом привязки к договорам/соглашения/актам по принципу FIFO. На форме можно выставить акт по одной или нескольким задолженностям в рамках одного договора.
