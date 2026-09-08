# Юрий Туманов — публикации и выступления
## Yuriy Tumanov — Publications and Talks

Актуально на 8 сентября 2026 года · As of 8 September 2026

---

## Профиль · Profile

**Туманов Юрий Михайлович** (Эльария, Psycho Drake) — кандидат технических наук, lead-эксперт по безопасности приложений в «Ростелекоме». В информационной безопасности с 2001 года. Выпускник НИЯУ МИФИ.

Текущая исследовательская линия — **ZeroFalse**: доказательный (evidence-first) триаж срабатываний статического анализа с помощью локальных языковых моделей. Модель не получает права на вердикт, пока не сошлётся на проверяемые улики в коде; при недостатке улик система честно отвечает `Unknown` и возвращает находку человеку. Стек экспериментов: Qwen2.5-Coder-14B-AWQ на vLLM, одна потребительская видеокарта с 16 ГБ VRAM.

> **Yuriy M. Tumanov** — Candidate of Technical Sciences, Lead Application Security expert at Rostelecom, in information security since 2001, MEPhI alumnus. Current research: evidence-anchored SAST triage with local LLMs inside a closed perimeter — a model may confirm a finding only when it cites verifiable evidence anchors, and must answer `Unknown` otherwise.

**LinkedIn:** https://www.linkedin.com/in/yury-tumanov-bb55b531/

**Направления · Focus areas**

| RU | EN |
|---|---|
| Evidence-first триаж SAST на локальных LLM | Evidence-anchored SAST triage with local LLMs |
| Снижение false positive в SAST / SCA / secret scanning без потери реальных находок | False-positive reduction without losing true findings |
| DevSecOps-автоматизация, качество правил анализаторов | DevSecOps automation, analyzer rule quality |
| Безопасность ИИ-агентов в закрытом контуре | Security controls for AI agents in restricted perimeters |

---

## Ключевые результаты · Headline results

- **746** срабатываний SAST, размеченных экспертами независимо от модели. Полное трёхклассовое совпадение — **47,5 %**; на 276 случаях, где содержательный вердикт вынесли и эксперт, и модель, — **80,8 %**; на пяти классах CWE, отобранных формальным правилом допуска, — **93,8 %** (150 из 160).
- **75 727** уникальных находок в ретроспективной выборке (нормализовано ~1,57 млн исторических записей): **precision 98,5 %**, recall 74,6 %, F1 0,85 для класса Confirmed при доле `Unknown` 9,6 %.
- Детерминированная дистилляция улик сокращает вход с **7 607** до **3 413** токенов, сохраняя совпадение 0,92 на решённых случаях.
- Формальное правило допуска класса дефектов к автоматизации: `D(c)=1`, если `n(c) ≥ 10`, `a(c) ≥ 0,75` и `m(c) ≥ 8`. Допуск прошли CWE-256, CWE-321, CWE-330, CWE-506, CWE-798.

---

## Выступления · Talks

### 2026

**ёPRSTCON 2026** (май 2026, трек locB «Магистраль») — **«От мешка false positive до нормального вердикта: паяем ZeroFalse-inspired LLM-триаж на локальных моделях»**. Видео, слайды и транскрипт: https://www.yoprstcon.ru/articles_manual_locB_html/11-zerofalse-llm-triage.html

**OFFZONE 2026** (20–21 августа 2026, Москва) — доклад по линии ZeroFalse: доказательный LLM-триаж SAST. Материалы: презентация, текст выступления, интервью-Q&A.

**STF Talks** (2026) — участие подтверждено официальным письмом организаторов.

### 2024

**Positive Hack Days 2024** — запись выступления: https://vk.com/video-28022322_456240844

### 2022

**OSday**, 24 июня 2022 — запись трансляции, выступление с 7:26:14: https://youtu.be/IZNjxJoBg-c?t=26776

### 2012 и ранее

**Защита кандидатской диссертации**, 2012 — запись: https://vk.com/video196891_167335441

**Microsoft, Санкт-Петербург, 2012** — работа «Methodic of destructive properties software verification for cloud computations» (верификация ПО на деструктивные свойства для облачных вычислений); сохранён диплом.

**Научная сессия НИЯУ МИФИ**, 2011 — доклад.

**Научная школа НИЯУ МИФИ**, 2010 — «Поведенческий анализ вредоносного кода, реализованного на языке JavaScript» / *Behaviour analysis of JavaScript malicious code*.

**Курчатовская молодёжная научная школа**, 2009 — «Использование поведенческого анализа для выявления вредоносного кода на примере JavaScript-сценариев»; доклад, презентация и публикация в сборнике.

**РусКрипто 2009** — участие: http://www.ruscrypto.org/sources/conference/rc2009/

**Инфофорум**, 26 января 2009 — участие: http://www.infoforum.ru/news/?p=628&n=819

*Требуют уточнения:* формат участия в мероприятии МИЭМП (2011) и год презентации «Сколково».

---

## Публикации · Publications

### 2026

**«Искусственный интеллект в арсенале нарушителя: анализ новых вызовов информационной безопасности»** — Коркин И. Ю., Туманов Ю. М., Докучаева О. Н. // «Вопросы кибербезопасности», № 4, 2026 (ВАК, РИНЦ). DOI: 10.21681/2311-3456-2026-4. Пройдены проверка на антиплагиат, экспертное заключение о возможности открытой публикации и оплата; в печати.

**"Weaponizing Intelligence: AI in the Hacker's Arsenal"** — Igor Korkin, Yuriy Tumanov, Oksana Dokuchaeva // eForensics Magazine, Vol. 13 No. 04, pp. 26–36. Опубликовано. Поверхности атаки на LLM: отравление контекста и вывод корпоративных данных через активные браузерные сессии пользователя.

**«Тесное окно: промпт-инжиниринг для локального триажа уязвимостей на одной видеокарте»** — журнал «Хакер», рубрика «Кодинг». Питч отправлен в редакцию; готовы карточка статьи и несколько редакций текста.

**«Звезда в машинном тумане»** — Хабр, лонгрид в соавторстве. Финальная редакция от 27.07.2026, иллюстрации готовы.

**ZeroFalse: доказательный LLM-триаж SAST** — Хабр, полный публикационный пакет (текст, иллюстрации, проверка метрик и ссылок). *Факт выхода уточнить.*

### 2009–2011 — журнал «Безопасность информационных технологий» (БИТ), НИЯУ МИФИ

**№ 4, 2011, с. 103–105** — статья сохранена постраничными сканами; *название уточнить*.

**№ 2, 2010, с. 83** — «Поиск уязвимостей по бинарному коду с помощью проверки выполнимости ограничений» / *Vulnerability detection in binary code based on constraint satisfiability checking*. Филоненко А. В., Исаев И. К., Сидоров Д. В., Туманов Ю. М. Тестирование на основе моделей, инструмент Avalanche (Valgrind + STP).

**№ 1, 2010** — «Использование поведенческого анализа с применением поведенческих сигнатур для выявления вредоносного кода на примере JavaScript-сценариев». Туманов Ю. М., Гаврилюк С. В. https://bit.mephi.ru/index.php/bit/article/view/791

**№ 1, 2010** — «Разработка метода защиты вычислительных Грид-сетей от намеренного искажения результата вычислений». Гаврилюк С. В., Туманов Ю. М.

**№ 4, 2009, с. 63** — «Обнаружение вредоносных сценариев JavaScript на основе поведенческих сигнатур». Туманов Ю. М.

**Сборник Курчатовской молодёжной научной школы, 2009** — «Использование поведенческого анализа для выявления вредоносного кода на примере JavaScript-сценариев».

---

## Заявки и подачи 2026 · Submission pipeline 2026

| Площадка · Venue | Работа · Work | Статус · Status |
|---|---|---|
| **IEEE ICCC 2026**, Чэнду, 11–14.12.2026 | *Evidence-Anchored LLM Triage for Static Application Security Testing in CI/CD Pipelines* (IC012) | Рецензия 39/60, подготовлены ревизия и Response to Reviewers |
| **CODE BLUE 2026** | *The Model Is Not the Verdict: Evidence-Anchored Local LLM Triage for SAST* · *Context Windows Lie: Engineering LLM Security Triage Under Real Memory and Evidence Constraints* | Два пакета подготовлены |
| **CCCI 2026** | *Evidence-Gated SAST Triage with Small Local LLMs: A ZeroFalse-Inspired Precision-First Pipeline* | Подано |
| **Pass the SALT 2026** | *Evidence, Not Guesswork: Precision-First SAST Triage with Self-Hosted Open LLMs* (short talk) | Подано |
| **РИ-2026**, СПб, 28–30.10.2026 | «Метод отбора классов дефектов для контролируемой автоматизации триажа SAST-срабатываний локальной языковой моделью» | Подано |
| **Positive Hack Days 2026** | «ZeroFalse: доказательный LLM-триаж SAST в CI/CD (precision-first без галлюцинаций)» | Подано |
| **Standoff Talks 2026** | ZeroFalse / LLM-триаж SAST | Подано |
| **ZeroNights 2026** | SAST + LLM (Qwen) | Подано |
| **No Hat 2026** | ZeroFalse | Пакет подготовлен |

---

## Исследовательские линии · Research lines

- **ZeroFalse / property-based triage** — вердикт по уликам, `Unknown` как безопасный отказ, post-валидация, CWE-специфичные политики, метрики precision / recall / unknown rate / dangerous misses.
- **Контекстное окно как архитектурное ограничение** — паспортное, операционное и полезное окно; бюджет промпта; лестница деградации, снимающая необязательные правила раньше улик.
- **AI в арсенале нарушителя** — классификация угроз, где ИИ одновременно инструмент атаки и её объект.
- **Безопасность ИИ-агентов** — OWASP Top 10 и OWASP LLM Top 10 применительно к продуктовой разработке; паттерны поведения агентов; оптимизация потребления токенов в агентных системах.

---

## Профили и ссылки · Profiles and links

- LinkedIn — https://www.linkedin.com/in/yury-tumanov-bb55b531/
- ёPRSTCON 2026, доклад — https://www.yoprstcon.ru/articles_manual_locB_html/11-zerofalse-llm-triage.html
- Positive Hack Days 2024, запись — https://vk.com/video-28022322_456240844
- OSday 2022, запись (с 7:26:14) — https://youtu.be/IZNjxJoBg-c?t=26776
- Защита кандидатской, 2012 — https://vk.com/video196891_167335441
- БИТ, статья 2010 — https://bit.mephi.ru/index.php/bit/article/view/791
