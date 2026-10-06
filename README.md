# Кристина Шишигина

**Бизнес-аналитик · BI-аналитика · Проектирование информационных систем**

Перевожу задачи предметной области в требования, пользовательские сценарии и модели данных. Соединяю анализ процессов с техническим пониманием системы и работой с продуктовыми метриками.

[Telegram][telegram] · [Email][email] · [Интерактивный дашборд][dashboard] · [Презентация «Ауры»][aura-slides]

## Обо мне

Я бизнес-аналитик с техническим бэкграундом и опытом стажировки в Яндекс Музыке. Работала с пользовательскими сценариями, аналитическими событиями и поведением приложения в критических состояниях.

В портфолио представлены два связанных кейса на примере «Ауры»: проектирование системы персонализированного подбора косметики и аналитика пользовательского пути в Power BI. Первый показывает работу с требованиями и устройством продукта, второй — определения метрик, модель отчётности и проверяемые гипотезы.

## Компетенции и инструменты

| Направление | С чем работаю | Пример в портфолио |
| --- | --- | --- |
| Требования | Анализ предметной области, декомпозиция, функциональные требования, бизнес-правила | [Спецификация][requirements] · [Бизнес-правила][business-rules] |
| Процессы и сценарии | AS-IS / TO-BE, IDEF0, UML, BPMN, CJM | [Процессы, IDEF0 и UML-сценарии «Ауры»][processes] |
| Данные и проектирование | SQL, PostgreSQL, модели данных, REST API | [Модель данных системы][aura-model] |
| BI и отчётность | Power BI, Power Query, DAX, ETL, продуктовые метрики | [Метрики][metrics] · [24 меры DAX][dax] |
| Анализ данных | Python, сравнение сегментов, визуализация, формулирование гипотез | [Аналитический разбор][findings] |

## Проекты

### AURA · Аналитика пользовательского пути в Power BI

**Бизнес-вопрос:** на каких этапах пользователи прекращают подбор, какие рекомендации добавляют в уход и какие изменения продукта стоит проверить?

[![Обзор продукта в Power BI: показатели и динамика пользовательского пути][powerbi-preview]][dashboard]

**[Открыть интерактивный дашборд →][dashboard]** · [Репозиторий][powerbi-repo] · [Скачать PBIX][pbix] · [Аналитический отчёт PDF][report-pdf]

В проекте определены KPI, подготовлена семантическая модель и реализованы 24 меры DAX. Пять страниц отчёта — «Обзор», «Пользователи», «Рекомендации», «Каталог» и «Воронка» — позволяют сравнивать периоды и сегменты, исследовать просмотры, добавления продуктов и сохранение ухода.

**Масштаб демонстрационного набора:** 8 000 пользователей, 120 продуктов, 60 000 рекомендаций; семь исходных CSV. На этих данных до заполнения профиля теряются 18,9% пользователей. Это основание для гипотезы об упрощении анкеты и исследования причин отказа.

Данные синтетические; выводы иллюстрируют метод анализа. Добавление продукта в уход не означает покупку, а улучшение бизнес-показателей после внедрения здесь не измерялось. Интерактивная версия на GitHub Pages — браузерная демонстрация на том же наборе данных. Отчёт и DAX-модель доступны в файле Power BI.

| Материал | Что можно посмотреть |
| --- | --- |
| [Определения метрик][metrics] | Числители, знаменатели и поведение фильтров |
| [Модель BI-данных][bi-model] | Таблицы, связи и временной контекст |
| [Меры DAX][dax] | Исходные формулы расчётов |
| [Выводы и гипотезы][findings] | Наблюдения, ограничения и следующие исследования |
| [Исходники PBIP][pbip] · [CSV-данные][data] | Материалы для изучения и воспроизведения отчёта |

**Инструменты:** Power BI Desktop, Power Query, DAX, CSV; HTML, CSS и JavaScript для браузерной демонстрации.

### АИС «Аура» · Дипломный проект

Информационная система персонализированного подбора косметических продуктов с учётом профиля пользователя, состава средств и базы знаний; консультационный чат использует RAG и векторный поиск.

**Мой вклад:** исследование предметной области, формирование требований, описание AS-IS / TO-BE и пользовательских сценариев, проектирование моделей данных и формализация логики рекомендаций.

**[Код и описание проекта →][aura-repo]** · [Презентация проекта][aura-slides] · [Видеопрезентация][aura-video] · [Полный текст ВКР][aura-thesis]

| Аналитический материал | Содержание |
| --- | --- |
| [Спецификация требований][requirements] | Назначение, границы, функции и ограничения системы |
| [Процессы и сценарии][processes] | Участники, AS-IS / TO-BE, сценарии пользователя и служебные процессы |
| [Модель данных][aura-model] | Концептуальная, логическая и физическая модели; PostgreSQL и Weaviate |
| [Бизнес-правила][business-rules] | Условия подбора, ограничения и расчёт совместимости |

<details>
<summary>Посмотреть схемы проекта: процесс TO-BE и концептуальную модель</summary>

**Персонализированный подбор с использованием системы — IDEF0 TO-BE.**

[![Контекстная диаграмма IDEF0 TO-BE системы «Аура»][process-preview]][process-preview]

[Описание процесса и его декомпозиция][processes]

**Концептуальная модель предметной области.**

[![Концептуальная модель данных системы «Аура»][model-preview]][model-preview]

[Сущности, связи и физическая реализация][aura-model]

</details>

**Технический контекст:** PostgreSQL, REST API, Weaviate, RAG; серверная часть, мобильное приложение и веб-интерфейс администрирования.

## Опыт

**Яндекс Музыка · Стажёр-разработчик**  
Сентябрь 2025 — январь 2026

- Проектировала разметку пользовательских событий и требования к мониторингу.
- Анализировала инциденты нехватки памяти и формализовала поведение приложения с учётом ограничений ОС.
- Описывала пользовательские сценарии и состояния при миграции системы управления профилем.
- Прорабатывала поведение интерфейса в зависимости от состояния приложения.

## Образование

**Московский политехнический университет**

- Бакалавриат: прикладная информатика, корпоративные информационные системы — 2026.
- Магистратура: прикладная математика и информатика, системная аналитика больших данных — ожидаемый год окончания 2028.
- Профессиональная переподготовка: нейросетевые технологии — 2024.

**Языки:** русский — родной; английский — B2.

## Связаться со мной

Открыта к предложениям в бизнес-анализе и BI-аналитике.

[Написать в Telegram][telegram] · [krishigina@yandex.ru][email]

[telegram]: https://t.me/krishigina
[email]: mailto:krishigina@yandex.ru
[dashboard]: https://kristinashishigina00.github.io/aura-powerbi/
[powerbi-repo]: https://github.com/KristinaShishigina00/aura-powerbi
[powerbi-preview]: https://raw.githubusercontent.com/KristinaShishigina00/aura-powerbi/main/assets/01-overview.png
[pbix]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/powerbi/Aura_Business_Analytics.pbix?raw=true
[pbip]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/powerbi/Aura_PBIP_Source.zip?raw=true
[report-pdf]: https://kristinashishigina00.github.io/aura-powerbi/report.pdf
[metrics]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/docs/metrics.md
[bi-model]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/docs/data-model.md
[dax]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/docs/dax-measures.md
[findings]: https://github.com/KristinaShishigina00/aura-powerbi/blob/main/docs/analytics-report.md
[data]: https://github.com/KristinaShishigina00/aura-powerbi/tree/main/data
[aura-repo]: https://github.com/KristinaShishigina00/Aura
[requirements]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/requirements.pdf
[processes]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/analysis/processes.md
[aura-model]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/analysis/data-model.md
[business-rules]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/analysis/business-rules.md
[aura-thesis]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/thesis.pdf
[aura-slides]: https://github.com/KristinaShishigina00/Aura/blob/master/docs/presentation.pdf
[aura-video]: https://youtu.be/Ott65TCBb2E
[process-preview]: https://raw.githubusercontent.com/KristinaShishigina00/Aura/master/docs/analysis/images/to-be-context.png
[model-preview]: https://raw.githubusercontent.com/KristinaShishigina00/Aura/master/docs/analysis/images/conceptual-model.png
