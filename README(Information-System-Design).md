[file name]: README(Information-System-Design).md
[file content begin]
# Information-System-Design — учебный проект бизнес/системного аналитика (BSA00–BSA11)

## Оглавление
- [1. Краткое описание проекта](#1-краткое-описание-проекта)
- [2. Цель проекта и бизнес-контекст](#2-цель-проекта-и-бизнес-контекст)
- [3. Стек и инструменты](#3-стек-и-инструменты)
- [4. Структура репозитория](#4-структура-репозитория)
  - [4.1. BSA00_Decomposition](#41-bsa00_decomposition)
  - [4.2. BSA01_Stakeholders](#42-bsa01_stakeholders)
  - [4.3. BSA02_Requirements](#43-bsa02_requirements)
  - [4.4. BSA03_HowToRequirements](#44-bsa03_howtorequirements)
  - [4.5. BSA04_Domains](#45-bsa04_domains)
  - [4.6. BSA05_Diagrams](#46-bsa05_diagrams)
  - [4.7. BSA06_BPMN](#47-bsa06_bpmn)
  - [4.8. BSA07_UserStory](#48-bsa07_userstory)
  - [4.9. BSA08_UseCase](#49-bsa08_usecase)
  - [4.10. BSA09_Objects-and-Roles](#410-bsa09_objects-and-roles)
  - [4.11. BSA10_FunctionalRequirements](#411-bsa10_functionalrequirements)
  - [4.12. BSA11_UserInterfaces](#412-bsa11_userinterfaces)
- [5. Артефакты бизнес-системного анализа](#5-артефакты-бизнес-системного-анализа)
- [6. Какие навыки бизнес-системного аналитика демонстрирует проект](#6-какие-навыки-бизнес-системного-аналитика-демонстрирует-проект)

---

## 1. Краткое описание проекта
Репозиторий содержит артефакты учебного проекта по анализу и проектированию информационной системы для двух предметных областей:
- **SNHC** — система онлайн-записи и обслуживания клиентов сети барбершопов (слоты услуг, мастера, клиенты, уведомления, скидки).
- **DLOR** — система обработки и доставки заказов (оператор/диспетчер/курьер, контроль статусов заказа).

В рамках курса выполнены ключевые артефакты системного/бизнес-анализа: декомпозиция, стейкхолдеры, требования as-is/to-be, модели данных, диаграммы процессов/состояний, BPMN, User Stories, Use Cases, объектная модель, UI-спецификация.

## 2. Цель проекта и бизнес-контекст
**Цель:** продемонстрировать полный цикл работ аналитика — от исследования предметной области и формализации требований до проектирования процессов, данных и интерфейсов.

**Бизнес-контекст SNHC:** автоматизация записи и управления слотами услуг, снижение ручных операций и ошибок.  
**Бизнес-контекст DLOR:** упорядочивание обработки заказов и доставки, прозрачное управление статусами и ролями.

## 3. Стек и инструменты
- Моделирование: **BPMN**, **UML**, **DFD**, **Swimlane**, **State diagram / State table**
- Данные: **ERD/логическая модель**, **Data Dictionary**, **CRUD matrix**
- Требования: **as-is/to-be**, **User Stories**, **Use Cases**
- UI: сценарии ролей, перечень экранов, **wireframes**, контроли/валидации
- Форматы: **PDF / SVG / PNG / JPG**

> В этом репозитории отсутствуют отдельные артефакты **SQL** и **Swagger/OpenAPI (YAML/JSON)**.

---

## 4. Структура репозитория

### 4.1. BSA00_Decomposition
**Фокус:** вход в предметную область, источники, глоссарии, декомпозиция.

- [`BSA00_Decomposition/DLOR/ex01_DLOR_infosources.pdf`](BSA00_Decomposition/DLOR/ex01_DLOR_infosources.pdf)  
  В рамках задания определены и зафиксированы источники информации по домену **DLOR** (какие артефакты/люди/документы используются для сбора требований).  
  Навыки: discovery, работа с источниками, формирование базы для elicitation.

- [`BSA00_Decomposition/DLOR/ex02_DLOR_glossary.pdf`](BSA00_Decomposition/DLOR/ex02_DLOR_glossary.pdf)  
  В рамках задания сформирован глоссарий терминов домена **DLOR**.  
  Навыки: терминологическое выравнивание, устранение неоднозначностей.

- [`BSA00_Decomposition/SNHC/ex01_SNHC_infosources.pdf`](BSA00_Decomposition/SNHC/ex01_SNHC_infosources.pdf)  
  В рамках задания определены источники информации по домену **SNHC**.  
  Навыки: discovery, подготовка к сбору требований.

- [`BSA00_Decomposition/SNHC/ex02_SNHC_glossary.pdf`](BSA00_Decomposition/SNHC/ex02_SNHC_glossary.pdf)  
  В рамках задания сформирован глоссарий терминов домена **SNHC**.  
  Навыки: управление терминологией.

- [`BSA00_Decomposition/ex03_decomposition.pdf`](BSA00_Decomposition/ex03_decomposition.pdf)  
  В рамках задания выполнена декомпозиция системы/проблемной области (структурирование на части/подсистемы/функции).  
  Навыки: системное мышление, разбиение сложности.

- [`BSA00_Decomposition/ex04_types.pdf`](BSA00_Decomposition/ex04_types.pdf)  
  В рамках задания описаны типы декомпозиции и их применение.  
  Навыки: методология анализа, выбор подхода к декомпозиции.

- [`BSA00_Decomposition/ex05_types.pdf`](BSA00_Decomposition/ex05_types.pdf)  
  В рамках задания продолжена работа с типами декомпозиции (закрепление на примере).  
  Навыки: практическое применение методологии.

- [`BSA00_Decomposition/ex06_rules.pdf`](BSA00_Decomposition/ex06_rules.pdf)  
  В рамках задания зафиксированы правила корректной декомпозиции и критерии качества разбиения.  
  Навыки: контроль качества аналитических артефактов.

---

### 4.2. BSA01_Stakeholders
**Фокус:** стейкхолдеры, окружение системы, потребности.

- [`BSA01_Stakeholders/ex00_DLOR_stakeholders.pdf`](BSA01_Stakeholders/ex00_DLOR_stakeholders.pdf)  
  В рамках задания составлен перечень стейкхолдеров системы **DLOR** с их ролями/интересами.  
  Навыки: stakeholder analysis, идентификация влияния.

- [`BSA01_Stakeholders/ex01_DLOR_onion.svg`](BSA01_Stakeholders/ex01_DLOR_onion.svg)  
  В файле построена **onion diagram** для **DLOR** (слои окружения: ядро/взаимодействующие/внешние).  
  Навыки: определение границ системы, контекстное моделирование.

- [`BSA01_Stakeholders/ex02_DLOR_needs.pdf`](BSA01_Stakeholders/ex02_DLOR_needs.pdf)  
  В рамках задания выявлены потребности/боли стейкхолдеров домена **DLOR**.  
  Навыки: elicitation, формулировка проблем и ожиданий.

- [`BSA01_Stakeholders/ex02_SNHC_needs.pdf`](BSA01_Stakeholders/ex02_SNHC_needs.pdf)  
  В рамках задания выявлены потребности/боли стейкхолдеров домена **SNHC**.  
  Навыки: elicitation, приоритизация потребностей.

- [`BSA01_Stakeholders/ex03_DLOR_glossary.pdf`](BSA01_Stakeholders/ex03_DLOR_glossary.pdf)  
  В рамках задания актуализирован глоссарий **DLOR** после анализа стейкхолдеров.  
  Навыки: управление изменениями терминологии.

- [`BSA01_Stakeholders/ex03_SNHC_glossary.pdf`](BSA01_Stakeholders/ex03_SNHC_glossary.pdf)  
  В рамках задания актуализирован глоссарий **SNHC** после анализа стейкхолдеров.  
  Навыки: согласование понятий между участниками.

---

### 4.3. BSA02_Requirements
**Фокус:** as-is/to-be, контекст, входные/выходные потоки.

- [`BSA02_Requirements/ex00_DLOR_asis.pdf`](BSA02_Requirements/ex00_DLOR_asis.pdf)  
  В рамках задания описаны роли и действия в текущем процессе (**as-is**) для **DLOR**.  
  Навыки: фиксация текущего состояния, выявление проблемных точек.

- [`BSA02_Requirements/ex00_SNHC_asis.pdf`](BSA02_Requirements/ex00_SNHC_asis.pdf)  
  В рамках задания описаны роли и действия (**as-is**) для **SNHC**.  
  Навыки: анализ текущих процессов.

- [`BSA02_Requirements/ex01_SNHC_context.svg`](BSA02_Requirements/ex01_SNHC_context.svg)  
  В файле описан контекст системы **SNHC** (внешние акторы/системы и взаимодействия).  
  Навыки: контекстное моделирование, границы системы.

- [`BSA02_Requirements/ex02_DLOR_tobe.pdf`](BSA02_Requirements/ex02_DLOR_tobe.pdf)  
  В рамках задания разработано целевое состояние (**to-be**) для **DLOR** с учетом проблем/потребностей.  
  Навыки: проектирование будущего процесса, формирование требований.

- [`BSA02_Requirements/ex02_SNHC_tobe.pdf`](BSA02_Requirements/ex02_SNHC_tobe.pdf)  
  В рамках задания разработано **to-be** для **SNHC**.  
  Навыки: улучшение процессов, формулировка целевых изменений.

- [`BSA02_Requirements/ex03_DLOR_streams.pdf`](BSA02_Requirements/ex03_DLOR_streams.pdf)  
  В рамках задания описаны входные/выходные потоки данных системы **DLOR**.  
  Навыки: data-flow thinking, подготовка к интеграциям/данным.

- [`BSA02_Requirements/ex03_SNHC_streams.pdf`](BSA02_Requirements/ex03_SNHC_streams.pdf)  
  В рамках задания описаны потоки данных **SNHC**.  
  Навыки: определение границ данных и взаимодействий.

- [`BSA02_Requirements/ex04_DLOR_glossary.pdf`](BSA02_Requirements/ex04_DLOR_glossary.pdf)  
  В рамках задания обновлен глоссарий **DLOR** по итогам требований.  
  Навыки: управление знаниями, согласование терминов.

- [`BSA02_Requirements/ex04_SNHC_glossary.pdf`](BSA02_Requirements/ex04_SNHC_glossary.pdf)  
  В рамках задания обновлен глоссарий **SNHC**.  
  Навыки: единая терминология требований.

---

### 4.4. BSA03_HowToRequirements
**Фокус:** техники выявления требований (DLOR), Vision.

- [`BSA03_HowToRequirements/ex00_DLOR_rolegame.pdf`](BSA03_HowToRequirements/ex00_DLOR_rolegame.pdf)  
  В рамках задания описана техника **role game** для выявления требований **SNHC** (сценарии взаимодействия ролей).  
  Навыки: facilitation, интервью/воркшопы, выявление требований через сценарии.

- [`BSA03_HowToRequirements/ex01_DLOR_brainstorming.pdf`](BSA03_HowToRequirements/ex01_DLOR_brainstorming.pdf)  
  В рамках задания зафиксированы результаты **brainstorming** (идеи/проблемы/гипотезы).  
  Навыки: генерация требований, структурирование идей.

- [`BSA03_HowToRequirements/ex02_DLOR_seminar.pdf`](BSA03_HowToRequirements/ex02_DLOR_seminar.pdf)  
  В рамках задания оформлены выводы **seminar** по требованиям.  
  Навыки: фасилитация обсуждений, фиксация решений.

- [`BSA03_HowToRequirements/ex03_DLOR_vision.pdf`](BSA03_HowToRequirements/ex03_DLOR_vision.pdf)  
  В файле сформирован документ **Vision** для **SNHC** (цели, контекст, ценность, границы).  
  Навыки: продуктовое мышление, формирование видения и scope.

---

### 4.5. BSA04_Domains
**Фокус:** сущности, CRUD-валидация, словарь данных, ER-модель.

- [`BSA04_Domains/ex00_DLOR_entity.pdf`](BSA04_Domains/ex00_DLOR_entity.pdf)  
  В рамках задания выделены сущности домена **DLOR**.  
  Навыки: domain modeling, выявление объектов предметной области.

- [`BSA04_Domains/ex00_SNHC_entity.pdf`](BSA04_Domains/ex00_SNHC_entity.pdf)  
  В рамках задания выделены сущности домена **SNHC**.  
  Навыки: domain modeling.

- [`BSA04_Domains/ex01_SNHC_crud.pdf`](BSA04_Domains/ex01_SNHC_crud.pdf)  
  В рамках задания построена CRUD-матрица для ключевых сущностей **SNHC**.  
  Навыки: валидация полноты требований, распределение операций по ролям/процессам.

- [`BSA04_Domains/ex02_DLOR_dict.pdf`](BSA04_Domains/ex02_DLOR_dict.pdf)  
  В рамках задания составлен словарь данных (атрибуты сущностей/справочников) для **DLOR**.  
  Навыки: спецификация данных, атрибутный уровень требований.

- [`BSA04_Domains/ex02_SNHC_dict.pdf`](BSA04_Domains/ex02_SNHC_dict.pdf)  
  В рамках задания составлен словарь данных для **SNHC**.  
  Навыки: data dictionary.

- [`BSA04_Domains/ex03_DLOR_model.pdf`](BSA04_Domains/ex03_DLOR_model.pdf)  
  В файле построена логическая модель данных (ERD) для **DLOR**.  
  Навыки: ERD/relationships, нормализация на уровне концепта.

- [`BSA04_Domains/ex03_SNHC_model.pdf`](BSA04_Domains/ex03_SNHC_model.pdf)  
  В файле построена логическая модель данных (ERD) для **SNHC**.  
  Навыки: проектирование данных.

---

### 4.6. BSA05_Diagrams
**Фокус:** DFD/Swimlane/State.

- [`BSA05_Diagrams/ex00_DLOR_dfd.png`](BSA05_Diagrams/ex00_DLOR_dfd.png)  
  В рамках задания построена DFD-диаграмма для **DLOR** (потоки данных и процессы).  
  Навыки: DFD, системное представление потоков.

- [`BSA05_Diagrams/ex00_SNHC_dfd.png`](BSA05_Diagrams/ex00_SNHC_dfd.png)  
  DFD для **SNHC**.  
  Навыки: DFD.

- [`BSA05_Diagrams/ex01_DLOR_swd.png`](BSA05_Diagrams/ex01_DLOR_swd.png)  
  Swimlane-диаграмма процесса **DLOR** (разделение по ролям/ответственности).  
  Навыки: моделирование процессов, RACI-like разделение ответственности.

- [`BSA05_Diagrams/ex01_SNHC_swd.png`](BSA05_Diagrams/ex01_SNHC_swd.png)  
  Swimlane для **SNHC**.  
  Навыки: процессный анализ.

- [`BSA05_Diagrams/ex02_DLOR_adswd.png`](BSA05_Diagrams/ex02_DLOR_adswd.png)  
  В рамках задания уточнена swimlane-диаграмма **DLOR** с артефактами/данными.  
  Навыки: повышение точности процесса, связка действий с данными.

- [`BSA05_Diagrams/ex02_SNHC_adswd.png`](BSA05_Diagrams/ex02_SNHC_adswd.png)  
  Аналогично для **SNHC**.  
  Навыки: детализация процессов.

- [`BSA05_Diagrams/ex03_DLOR_dst.png`](BSA05_Diagrams/ex03_DLOR_dst.png)  
  В рамках задания построена диаграмма состояний (state diagram) для объекта домена **DLOR**.  
  Навыки: жизненный цикл сущностей, статусы и переходы.

- [`BSA05_Diagrams/ex03_SNHC_dst.png`](BSA05_Diagrams/ex03_SNHC_dst.png)  
  Диаграмма состояний для **SNHC**.  
  Навыки: state modeling.

- [`BSA05_Diagrams/ex04_DLOR_tst.pdf`](BSA05_Diagrams/ex04_DLOR_tst.pdf)  
  В рамках задания оформлена таблица состояний (state transition table) для **DLOR**.  
  Навыки: формализация переходов, условия, события.

- [`BSA05_Diagrams/ex04_SNHC_tst.pdf`](BSA05_Diagrams/ex04_SNHC_tst.pdf)  
  Таблица состояний для **SNHC**.  
  Навыки: проверяемость логики статусов.

---

### 4.7. BSA06_BPMN
**Фокус:** BPMN-процессы DLOR + согласование/ревизия.

- [`BSA06_BPMN/ex00_DLOR_base_information.pdf`](BSA06_BPMN/ex00_DLOR_base_information.pdf)  
  В рамках задания собрана базовая информация для моделирования процессов **DLOR** (контекст/участники/объекты).  
  Навыки: подготовка BPMN, сбор исходных данных.

- [`BSA06_BPMN/ex00_SNHC_base_information.pdf`](BSA06_BPMN/ex00_SNHC_base_information.pdf)  
  Базовая информация для **SNHC**.  
  Навыки: подготовка к моделированию.

- [`BSA06_BPMN/ex01_DLOR_mpr.pdf`](BSA06_BPMN/ex01_DLOR_mpr.pdf)  
  В рамках задания определен перечень основных бизнес-процессов **DLOR**.  
  Навыки: выделение процессов, декомпозиция по value stream.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp01_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp01_disc.pdf)  
  В рамках задания оформлено обсуждение/уточнения процесса BPMN №1 (замечания, вопросы, согласование).  
  Навыки: коммуникации, протоколирование, работа с обратной связью.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp02_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp02_disc.pdf)  
  Обсуждение процесса BPMN №2.  
  Навыки: согласование артефактов.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp03_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp03_disc.pdf)  
  Обсуждение процесса BPMN №3.  
  Навыки: управление изменениями.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp04_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp04_disc.pdf)  
  Обсуждение процесса BPMN №4.  
  Навыки: уточнение требований через процесс.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp05_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp05_disc.pdf)  
  Обсуждение процесса BPMN №5.  
  Навыки: согласование.

- [`BSA06_BPMN/ex02/ex02_DLOR_bp06_disc.pdf`](BSA06_BPMN/ex02/ex02_DLOR_bp06_disc.pdf)  
  Обсуждение процесса BPMN №6.  
  Навыки: согласование.

- [`BSA06_BPMN/ex03_DLOR_mpr.pdf`](BSA06_BPMN/ex03_DLOR_mpr.pdf)  
  В рамках задания описаны основные бизнес-процессы **DLOR** (текстовое описание/границы/участники).  
  Навыки: спецификация процессов.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp01.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp01.jpg)  
  В рамках задания построена BPMN-диаграмма процесса **DLOR** №1.  
  Навыки: BPMN notation, события/шлюзы/сообщения.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp02.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp02.jpg)  
  BPMN процесса №2.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp03.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp03.jpg)  
  BPMN процесса №3.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp04.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp04.jpg)  
  BPMN процесса №4.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp05.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp05.jpg)  
  BPMN процесса №5.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex04/ex04_barb_bpmn_bp06.jpg`](BSA06_BPMN/ex04/ex04_barb_bpmn_bp06.jpg)  
  BPMN процесса №6.  
  Навыки: BPMN.

- [`BSA06_BPMN/ex05_DLOR_glossary.pdf`](BSA06_BPMN/ex05_DLOR_glossary.pdf)  
  В рамках задания выполнена актуализация глоссария **DLOR** после BPMN.  
  Навыки: консистентность терминов между процессами и требованиями.

- [`BSA06_BPMN/ex05_DLOR_rev.pdf`](BSA06_BPMN/ex05_DLOR_rev.pdf)  
  В рамках задания проведена ревизия артефактов **DLOR** по итогам обсуждений и BPMN.  
  Навыки: quality review, управление изменениями, выравнивание артефактов.

---

### 4.8. BSA07_UserStory
**Фокус:** User Stories (SNHC).

- [`BSA07_UserStory/ex00_SNHC_us_manager_.pdf`](BSA07_UserStory/ex00_SNHC_us_manager_.pdf)  
  В рамках задания сформированы User Stories для роли **Manager** в домене **SNHC**.  
  Навыки: user-centric требования, ценность/цель, критерии приемки.

- [`BSA07_UserStory/ex01_SNHC_us_роль_.pdf`](BSA07_UserStory/ex01_SNHC_us_роль_.pdf)  
  В рамках задания сформированы User Stories для ролей: Client / Master.  
  Навыки: покрытие ролей, согласование ожиданий разных пользователей.

- [`BSA07_UserStory/ex02_HAIR_us.pdf`](BSA07_UserStory/ex02_HAIR_us.pdf)  
  В рамках задания оформлен итоговый документ по User Stories (компоновка/согласование/протокол).  
  Навыки: консолидация требований, управление набором US.

---

### 4.9. BSA08_UseCase
**Фокус:** Use Cases (SNHC).

- [`BSA08_UseCase/ex00_SNHC_UC.pdf`](BSA08_UseCase/ex00_SNHC_UC.pdf)  
  В рамках задания описаны Use Cases SNHC (набор UC и/или основной сценарий).  
  Навыки: формализация сценариев, акторы, предусловия/постусловия.

- [`BSA08_UseCase/ex01_SNHC_UC.pdf`](BSA08_UseCase/ex01_SNHC_UC.pdf)  
  Use Case документ №2 (детализация/дополнение UC).  
  Навыки: альтернативные потоки, исключения.

- [`BSA08_UseCase/ex02_SNHC_UC.pdf`](BSA08_UseCase/ex02_SNHC_UC.pdf)  
  Use Case документ №3.  
  Навыки: полнота сценариев.

- [`BSA08_UseCase/ex03_SNHC_UC.pdf`](BSA08_UseCase/ex03_SNHC_UC.pdf)  
  Use Case документ №4.  
  Навыки: согласование бизнес-правил через сценарии.

- [`BSA08_UseCase/ex04_SNHC_UC.pdf`](BSA08_UseCase/ex04_SNHC_UC.pdf)  
  Use Case документ №5.  
  Навыки: трассировка к объектам/статусам.

- [`BSA08_UseCase/ex05_SNHC_UC.pdf`](BSA08_UseCase/ex05_SNHC_UC.pdf)  
  Use Case документ №6 (закрытие набора UC).  
  Навыки: систематизация UC.

---

### 4.10. BSA09_Objects-and-Roles
**Фокус:** объекты, роли, классы (HSR).

- [`BSA09_Objects and Roles/Exercise_00_Persona.pdf`](BSA09_Objects%20and%20Roles/Exercise_00_Persona.pdf)  
  В рамках задания выделены классы/сущности для персон (пользователи/персоны) в системе HSR.  
  Навыки: объектное моделирование, атрибуты, роли.

- [`BSA09_Objects and Roles/Exercise_01_Clients_Employees.pdf`](BSA09_Objects%20and%20Roles/Exercise_01_Clients_Employees.pdf)  
  В рамках задания описаны сущности клиентов и сотрудников, их различия и атрибуты.  
  Навыки: моделирование ролей и прав, доменная сегментация.

- [`BSA09_Objects and Roles/Exercise_02_Employee_Services_Master.pdf`](BSA09_Objects%20and%20Roles/Exercise_02_Employee_Services_Master.pdf)  
  В рамках задания описаны справочники и сущности, связанные с ними.  
  Навыки: reference data, классификаторы.

- [`BSA09_Objects and Roles/Exercise_03_Service_Slots.pdf`](BSA09_Objects%20and%20Roles/Exercise_03_Service_Slots.pdf)  
  В рамках задания описан объект “слот услуги” и связанные атрибуты/состояния/операции.  
  Навыки: анализ ключевого объекта, подготовка к статусной модели и CRUD.

- [`BSA09_Objects and Roles/Exercise_04_Class_Diagram.png`](BSA09_Objects%20and%20Roles/Exercise_04_Class_Diagram.png)  
  В файле построена UML class diagram (классы и связи).  
  Навыки: UML, связи/агрегации, целостность модели.

- [`BSA09_Objects and Roles/Exercise_05_Discounts,Notification.pdf`](BSA09_Objects%20and%20Roles/Exercise_05_Discounts,Notification.pdf)  
  В рамках задания выделены сущности скидок и уведомлений и их место в модели.  
  Навыки: расширение модели, учет бизнес-правил.

- [`BSA09_Objects and Roles/Exercise_06_Class_Diagram.png`](BSA09_Objects%20and%20Roles/Exercise_06_Class_Diagram.png)  
  В файле представлена итоговая диаграмма (модель/связи) после уточнений.  
  Навыки: итеративное улучшение модели.

---

### 4.11. BSA10_FunctionalRequirements
**Фокус:** функциональные требования, статусы, CRUD, права.

- [`BSA10_FunctionalRequirements/Exercise_00_objects.pdf`](BSA10_FunctionalRequirements/Exercise_00_objects.pdf)  
  В рамках задания определены объекты, для которых требуется статусная модель.  
  Навыки: выделение управляемых сущностей, подготовка статусов.

- [`BSA10_FunctionalRequirements/Exercise_01_Life_Cycle_of_the_Service_slots.pdf`](BSA10_FunctionalRequirements/Exercise_01_Life_Cycle_of_the_Service_slots.pdf)  
  В рамках задания описан жизненный цикл объекта “слот услуги”.  
  Навыки: state lifecycle, события и переходы.

- [`BSA10_FunctionalRequirements/Exercise_02_Status_models_of_the_entety.pdf`](BSA10_FunctionalRequirements/Exercise_02_Status_models_of_the_entety.pdf)  
  В рамках задания разработаны статусные модели для сущностей системы.  
  Навыки: формализация статусов, условия переходов.

- [`BSA10_FunctionalRequirements/Exercise_03_Description_of_actions_on_References.pdf`](BSA10_FunctionalRequirements/Exercise_03_Description_of_actions_on_References.pdf)  
  В рамках задания описаны действия над справочниками/референсными данными.  
  Навыки: CRUD для справочников, администрирование данных.

- [`BSA10_FunctionalRequirements/Exercise_04_CRUD_Operations_on_the_Service_Slots_Object.pdff`](BSA10_FunctionalRequirements/Exercise_04_CRUD_Operations_on_the_Service_Slots_Object.pdf)  
  В рамках задания определены CRUD-операции над “слотом услуги”.  
  Навыки: детализация операций, права/ограничения.

- [`BSA10_FunctionalRequirements/Exercise_05_Detailed_Operations_on_the_Service_Slots_Object.pdf`](BSA10_FunctionalRequirements/Exercise_05_Detailed_Operations_on_the_Service_Slots_Object.pdf)  
  В рамках задания детализированы операции над объектом “слот услуги” (условия, проверки, эффекты).  
  Навыки: спецификация логики, проверяемость.

- [`BSA10_FunctionalRequirements/Exercise_06_Role_Access_Rights.pdf`](BSA10_FunctionalRequirements/Exercise_06_Role_Access_Rights.pdf)  
  В рамках задания определены права доступа по ролям.  
  Навыки: RBAC, безопасность на уровне требований.

---

### 4.12. BSA11_UserInterfaces
**Фокус:** UI-спецификация, сценарии, wireframes.

- [`BSA11_UserInterfaces/Exercise_00_Choosing_the_Form_of_Product_Presentation.pdf`](BSA11_UserInterfaces/Exercise_00_Choosing_the_Form_of_Product_Presentation.pdf)  
  В рамках задания определен подход к представлению продукта/данных в интерфейсе.  
  Навыки: UX-логика, выбор формы подачи информации.

- [`BSA11_UserInterfaces/Exercise_01_Creation_Forms_of_Classifiers_and_References.pdf`](BSA11_UserInterfaces/Exercise_01_Creation_Forms_of_Classifiers_and_References.pdf)  
  В рамках задания описаны экранные формы для классификаторов и справочников.  
  Навыки: проектирование админ-интерфейсов.

- [`BSA11_UserInterfaces/Exercise_02_Data_on_the_Screen_Forms_of_Classifiers_and_References.pdf`](BSA11_UserInterfaces/Exercise_02_Data_on_the_Screen_Forms_of_Classifiers_and_References.pdf)  
  В рамках задания определены данные/поля, отображаемые на формах.  
  Навыки: data-to-UI mapping, спецификация полей.

- [`BSA11_UserInterfaces/Exercise_03_Key_Role_Scenarios.pdf`](BSA11_UserInterfaces/Exercise_03_Key_Role_Scenarios.pdf)  
  В рамках задания описаны ключевые сценарии ролей в UI.  
  Навыки: user flow, приоритизация сценариев.

- [`BSA11_UserInterfaces/Exercise_04_List_of_Screen_Forms.pdf`](BSA11_UserInterfaces/Exercise_04_List_of_Screen_Forms.pdf)  
  В рамках задания составлен перечень экранных форм.  
  Навыки: UI inventory, coverage.

- [`BSA11_UserInterfaces/ex05/Exercise_05_Master_Schedule_(wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise_05_Master_Schedule_(wireframe).pdf)  
  В рамках задания создан wireframe экрана расписания мастера.  
  Навыки: wireframing, UX для расписаний/слотов.

- [`BSA11_UserInterfaces/ex05/Exercise_05_Preview_Your_Own_Schedule_(wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise_05_Preview_Your_Own_Schedule_(wireframe).pdf)  
  Wireframe просмотра собственного расписания.  
  Навыки: UX сценарии пользователя.

- [`BSA11_UserInterfaces/ex05/Exercise_05_Slot_Reservation(wireframe).pdf`](BSA11_UserInterfaces/ex05/Exercise_05_Slot_Reservation(wireframe).pdf)  
  Wireframe бронирования слота.  
  Навыки: UX критического сценария “запись”.

- [`BSA11_UserInterfaces/Exercise_06_Controls_Description.pdf`](BSA11_UserInterfaces/Exercise_06_Controls_Description.pdf)  
  В рамках задания описаны элементы управления, проверки, ограничения ввода.  
  Навыки: UI-валидации, нефункциональные аспекты удобства/ошибок.

---

## 5. Артефакты бизнес-системного анализа
- Требования (as-is/to-be): [`BSA02_Requirements/*`](BSA02_Requirements/)
- Стейкхолдеры и контекст: [`BSA01_Stakeholders/*`](BSA01_Stakeholders/), [`BSA02_Requirements/ex01_SNHC_context.svg`](BSA02_Requirements/ex01_SNHC_context.svg)
- BPMN / процессная модель: [`BSA06_BPMN/*`](BSA06_BPMN/)
- UML / объектная модель: [`BSA09_Objects and Roles/*`](BSA09_Objects%20and%20Roles/)
- ERD / модель данных и словари: [`BSA04_Domains/*`](BSA04_Domains/)
- Диаграммы потоков и состояний: [`BSA05_Diagrams/*`](BSA05_Diagrams/)
- User Stories: [`BSA07_UserStory/*`](BSA07_UserStory/)
- Use Cases: [`BSA08_UseCase/*`](BSA08_UseCase/)
- Функциональная детализация (статусы/CRUD/права): [`BSA10_FunctionalRequirements/*`](BSA10_FunctionalRequirements/)
- UI-спецификация и wireframes: [`BSA11_UserInterfaces/*`](BSA11_UserInterfaces/)

## 6. Какие навыки бизнес-системного аналитика демонстрирует проект
- Анализ предметной области: декомпозиция, глоссарий, сущности
- Стейкхолдер-анализ: карта окружения (onion), потребности/боли
- Формализация требований: as-is/to-be, user stories, use cases
- Процессное моделирование: DFD, swimlane, BPMN
- Моделирование данных: ERD, data dictionary, CRUD-валидация
- Проектирование функциональности: статусы, CRUD-операции, RBAC
- UI-аналитика: сценарии, перечень экранов, wireframes, контроли/валидации
[file content end]
