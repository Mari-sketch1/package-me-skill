# Package Me

`package-me` — интерактивный навык для упаковки многогранного личного бренда в Telegram, VK и Instagram на основе `UNPACKING_DOSSIER.md`.

Он строит audience-first вход и person-first глубину: первый экран дает незнакомому человеку понятную причину остаться, не сводя автора к одной боли, роли или маркетинговой нише.

## Что делает навык

- собирает карту граней, доказательств и публичных границ;
- сравнивает несколько архитектур личного бренда;
- строит audience entry doors и disclosure ladder;
- создает разные по механике варианты названий и bio;
- проверяет первый экран на холодной аудитории;
- формирует голос, контентную архитектуру и визуальное направление;
- адаптирует упаковку отдельно для Telegram, VK и Instagram;
- создает `PACKAGING_DECISIONS.md` и `SOCIAL_PACKAGING.md`.

## Установка в Codex

### Для всех проектов пользователя

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/Mari-sketch1/package-me-skill.git ~/.codex/skills/package-me
```

После установки перезапустите Codex и вызовите навык:

```text
$package-me
```

### Только для одного проекта

Выполните из корня проекта:

```bash
mkdir -p .codex/skills
git clone https://github.com/Mari-sketch1/package-me-skill.git .codex/skills/package-me
```

## Установка в Claude Code

### Для всех проектов пользователя

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/Mari-sketch1/package-me-skill.git ~/.claude/skills/package-me
```

После установки перезапустите Claude Code и вызовите навык:

```text
/package-me
```

### Только для одного проекта

Выполните из корня проекта:

```bash
mkdir -p .claude/skills
git clone https://github.com/Mari-sketch1/package-me-skill.git .claude/skills/package-me
```

Project skill можно сохранить в Git, чтобы он был доступен всей команде и в Claude Code cloud sessions.

## Обновление

Codex:

```bash
git -C ~/.codex/skills/package-me pull --ff-only
```

Claude Code:

```bash
git -C ~/.claude/skills/package-me pull --ff-only
```

## Входные данные

Основной вход — `UNPACKING_DOSSIER.md`, созданный после глубокой распаковки личности. Если досье имеет другое имя, укажите его при запуске.

Навык работает в интерактивном Guided mode по умолчанию. Fast mode включается только по прямой просьбе выполнить упаковку без промежуточных выборов.

## Структура

```text
package-me/
├── SKILL.md
└── references/
    ├── COPY_LAB.md
    ├── CREATIVE_VARIATION_LAB.md
    ├── EVALS.md
    ├── INPUT_CONTRACT.md
    ├── INTERACTIVE_WORKFLOW.md
    ├── OUTPUT_TEMPLATE.md
    ├── PACKAGING_MODEL.md
    ├── PLATFORM_PLAYBOOKS.md
    ├── POSITIONING_LAB.md
    ├── QUALITY_BAR.md
    └── SPIRITUAL_INTEGRITY.md
```

## Совместимость

Навык использует открытый формат Agent Skills: каталог с `SKILL.md`, YAML frontmatter и дополнительными файлами в `references/`.

- [OpenAI: Skills](https://developers.openai.com/api/docs/guides/tools-skills)
- [Claude Code: Skills](https://code.claude.com/docs/en/skills)

Текущая версия: **4.2**.
