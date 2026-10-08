# Портфолио системного аналитика — School 21 (Сбер)

Артефакты системного анализа, выполненные в рамках трека «Системный анализ» School 21 (Сбер) — от сбора требований до моделирования данных и бизнес-процессов. 

**Арег Дерцян**
<br>✉️ areg.abraamyan.0@mail.ru <br> 💬 [Telegram](https://t.me/AVanLore)

---

## Содержание

| Навык | Артефакт | Комментарий |
|---|---|---|
| BPMN | [Cправочники](diagrams/BPMN/bbs-bpmn-ref.png) · [Расписание](diagrams/BPMN/bbs-bpmn-sch.png) · [Запись на услугу](diagrams/BPMN/bbs-bpmn-book.png) · [Учёт и оплата](diagrams/BPMN/bbs-bpmn-bill.png) | 4 процесса в порядке работы системы |
| UML, диаграмма классов | [bbs-class-diagram.png](diagrams/bbs-class-diagram.png) | итоговая модель данных |
| UML, диаграмма состояний | [bbs-state-diagram.png](diagrams/bbs-state-diagram.png) | жизненный цикл слота записи |
| DFD | [bbs-dfd.png](diagrams/bbs-dfd.png) | потоки данных, to be |
| ER-диаграмма | [bbs-erd.png](diagrams/bbs-erd.png) | ранняя концептуальная модель, см. раздел «Как ориентироваться» |
| Swimlane | [bbs-swimlane.png](diagrams/bbs-swimlane.png) | кросс-функциональный процесс записи |
| Use Cases | [клиент](use-cases/bbs-uc-client.md) · [менеджер](use-cases/bbs-uc-manager.md) · [мастер](use-cases/bbs-uc-master.md) | include/extend, альтернативные потоки |
| User Stories | [клиент](user-stories/bbs-us-client.md) · [менеджер](user-stories/bbs-us-manager.md) · [мастер](user-stories/bbs-us-master.md) | Given-When-Then + тестовые сценарии |
| CRUD / ролевая модель доступа | [bbs-crud-access-matrix.md](requirements/bbs-crud-access-matrix.md) | права, бизнес-правила, уведомления, журналирование |
| Нефункциональные требования | [bbs-nfr.md](requirements/bbs-nfr.md) | производительность, доступность, масштабируемость, безопасность |
| Сбор требований, стейкхолдеры | [dlvr-stakeholders.md](requirements/dlvr-stakeholders.md) · [луковичная диаграмма](diagrams/dlvr-onion-diagram.png) | доп. кейс «Доставка» |
| Vision / BRD | [dlvr-vision.md](requirements/dlvr-vision.md) | доп. кейс «Доставка» |

---

## Два кейса

| Кейс | Артефакты | Статус |
|---|---|---|
| **Барбершоп — онлайн-запись** (`bbs-`) | диаграммы, use cases, user stories, CRUD, НФТ | основной, сквозной |
| **Доставка заказов** (`dlvr-`) | стейкхолдеры, Vision | дополнительный пример |

Разные учебные задачи курса, не части одной системы.

---

## Как ориентироваться по репозиторию

Для кейса «Барбершоп», чтобы сложилась полная картина проекта, артефакты лучше смотреть в таком порядке:

1. [ERD](diagrams/bbs-erd.png) и [диаграмма классов](diagrams/bbs-class-diagram.png) — модель данных (ERD — ранняя версия, диаграмма классов — финальная; расхождения между ними — нормальная эволюция понимания предметной области, не ошибка).
2. [DFD](diagrams/bbs-dfd.png) — как данные движутся между участниками и системой.
3. [BPMN](diagrams/BPMN/) — сами бизнес-процессы, в порядке работы системы: [справочники](diagrams/BPMN/bbs-bpmn-ref.png) → [расписание](diagrams/BPMN/bbs-bpmn-sch.png) → [запись на услугу](diagrams/BPMN/bbs-bpmn-book.png) → [учёт и оплата](diagrams/BPMN/bbs-bpmn-bill.png).
4. [Swimlane](diagrams/bbs-swimlane.png) и [диаграмма состояний](diagrams/bbs-state-diagram.png) — детализация процесса записи и жизненного цикла слота.
5. [Use Cases](use-cases/) и [User Stories](user-stories/) — те же сценарии с точки зрения ролей.
6. [CRUD-матрица](requirements/bbs-crud-access-matrix.md) и [НФТ](requirements/bbs-nfr.md) — права доступа, бизнес-правила, требования к качеству.

Для кейса «Доставка» порядок проще: [каталог стейкхолдеров](requirements/dlvr-stakeholders.md) → [луковичная диаграмма](diagrams/dlvr-onion-diagram.png) → [Vision](requirements/dlvr-vision.md).
