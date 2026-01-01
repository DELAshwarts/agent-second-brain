# Entry Classification

<!--

-->

## Work Domains → Categories

Based on user's work context (see [ABOUT.md](ABOUT.md)):

### Client Work
Брифы, стратегии, креатив, кампании, KPI, предложения

<!-- Добавьте имена ваших клиентов через запятую -->
**Keywords:** [Джойнт, Адаин Ло, РЕК Москва, РЕК СПб, Сохнут, Голландцы, доноры, партнеры], клиент, бриф, презентация, дедлайн, KPI

**→ Category:** task (p1-p2) → Todoist

### AI & Tech
Инструменты, модели, промпты, пайплайны, агенты

**Keywords:** GPT, Claude, модель, агент, API, пайплайн, автоматизация, интеграция

**→ Category:** learning или project → thoughts/

### Product
Идеи, гипотезы, MVP, юнит-экономика

**Keywords:** продукт, SaaS, MVP, гипотеза, монетизация, юнит-экономика, стартап

**→ Category:** idea или project → thoughts/

### Company Ops
Команда, процессы, автоматизация, найм, управление, финансы

<!-- Замените [Your Company] на название вашей компании/проекта -->
**Keywords:** команда, найм, процесс, HR, финансы, [Фонд "Ресурсный центр еврейского просвещения"]

**→ Category:** task или project (depends on urgency)

### Content
Посты, идеи, тезисы для Telegram 

<!-- Замените [@your_channel] на ваш Telegram-канал или удалите если не нужно -->
**Keywords:** пост, [@havura_rc], контент, тезис, статья

**→ Category:** idea → thoughts/ideas/ или task если с дедлайном

---

## Decision Tree

```
Entry text contains...
│
├─ Client brand or deadline? ────────────────────> TASK (p1-p2)
│  ([Your Clients], клиент, дедлайн, презентация)
│
├─ Operational/urgent? ──────────────────────────> TASK (p2-p3)
│  (нужно сделать, не забыть, позвонить, встреча)
│
├─ AI/tech learning? ────────────────────────────> LEARNING
│  (узнал, модель, агент, интеграция)
│
├─ Product/SaaS idea? ───────────────────────────> IDEA или PROJECT
│  (продукт, MVP, гипотеза, SaaS)
│
├─ Strategic thinking? ──────────────────────────> PROJECT
│  (стратегия, план, R&D, долгосрочно)
│
├─ Personal insight? ────────────────────────────> REFLECTION
│  (понял, осознал, философия)
│
└─ Content idea? ────────────────────────────────> IDEA
   (пост, тезис, контент)
```

## Apply Decision Filters

Перед сохранением спроси:
- Это масштабируется?
- Это можно автоматизировать?
- Это усиливает экспертизу или бренд?
- Это приближает к продукту или SaaS?

Если да на 2+ вопроса → повысить приоритет.

---

## Photo Entries

For `[photo]` entries:

1. Analyze image content via vision
2. Determine domain:
   - Screenshot клиентского материала → Client Work
   - Схема/диаграмма → AI & Tech или Product
   - Текст/статья → Learning
3. Add description to daily file

---

## Output Locations

| Category | Destination | Priority |
|----------|-------------|----------|
| task (client) | Todoist | p1-p2 |
| task (ops) | Todoist | p2-p3 |
| task (content) | Todoist | p3-p4 |
| idea | thoughts/ideas/ | — |
| reflection | thoughts/reflections/ | — |
| project | thoughts/projects/ | — |
| learning | thoughts/learnings/ | — |

---

## File Naming

```
thoughts/{category}/{YYYY-MM-DD}-short-title.md
```

Examples:
```
thoughts/ideas/2024-12-16-saas-pricing-model.md
thoughts/projects/2024-12-16-ai-agents-pipeline.md
thoughts/learnings/2024-12-16-claude-mcp-setup.md
```

---

## Thought Structure

Use preferred format:

```markdown
---
date: {YYYY-MM-DD}
type: {category}
domain: {Client Work|AI & Tech|Product|Agency Ops|Content}
tags: [tag1, tag2]
---

## Context
[Что привело к мысли]

## Insight
[Ключевая идея]

## Implication
<!-- Замените [Your Company] на название вашей компании -->
[Что это значит для [Фонд "Ресурсный центр еврейского просвещения"]/продукта/стратегии]

## Next Action
[Конкретный шаг — не абстрактный]
```

---

## Anti-Patterns (ИЗБЕГАТЬ)

При создании мыслей НЕ делать:
- Абстрактные рассуждения без Next Action
- Академическая теория без применения к вашему проекту/продукту
- Повторы без синтеза (кластеризуй похожие!)
- Хаотичные списки без приоритетов
- Задачи типа "подумать о..." (конкретизируй!)

---

## MOC Updates

After creating thought file, add link to:
```
MOC/MOC-{category}s.md
```

Group by domain when relevant:
```markdown
## AI & Automation
- [[ai-grantwriter]] — ИИ-грантрайтер для заявок и отчетов
- [[ai-project-manager]] — управление сроками, рисками и задачами команды
- [[automation-docs]] — договоры, согласия, отчёты, шаблоны

## Strategy & Governance
- [[strategy-2025-2030]] — стратегические цели фонда
- [[decision-filters]] — управленческие фильтры и критерии выбора
- [[governance-model]] — роли, ответственность, контроль исполнения

## Projects & Events
- [[project-august-conference]] — Августовская конференция для педагогов еврейского образования
- [[project-bama]] — конференция «Бама»
- [[project-festival-knowledge]] — Фестиваль еврейских знаний / День еврейских знаний
- [[project-erudaika]] — Эрудаика (игры, олимпиады, форматы)
- [[fundament-pedagogue]] — «Фундамент для педагога»
- [[judaica-for-all]] — «Иудаика для каждого»

## Legal & Compliance
- [[pd-policy]] — персональные данные
- [[contracts-templates]] — договоры, акты, приложения, ТЗ
- [[grant-requirements]] — требования фондов и отчётность 

## Education & Content
- [[havura-library]] — библиотека методических материалов «Хавура» (архитектура, пополнение, редактура)
- [[pajama-library]] — «Пижамная библиотечка» (контент, партнёры, логистика, метрики)
- [[content-standards]] — стиль, тон, методика, редакционные правила

## Operations & Personal Effectiveness
- [[weekly-review]] — еженедельный обзор
- [[anti-chaos]] — правила против авралов
- [[energy-management]] — управление нагрузкой и восстановление
```
