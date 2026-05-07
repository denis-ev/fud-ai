# Play Store Listing

Google Play Console listing copy for Fud AI Android (current: v1.0.11 / versionCode 14). Each field is in a code block for easy copy-paste. Char counts are tracked because Play Console enforces hard caps and silently truncates anything over.

**Where to paste each field in Play Console:**
- App name / Short description / Full description → Grow → Store presence → **Main store listing** (default English) and Grow → Store presence → **Custom store listings** → Manage translations (per-language overrides)
- What's new → **Releases → Production / Closed testing → Create new release → Release notes** field (paste the entire `<lang-tag>` block; Play Console parses tags automatically)

---

## 1. App Name

**30 char hard cap per language.** Brand name stays as `Fud AI` untranslated; the descriptor after the dash is what gets localized. English-only on Play Console — non-English Play Store browsers see the English source as fallback.

### English (en-US) — 24 chars
```
Fud AI - Calorie Tracker
```

---

## 2. Short Description

**80 char hard cap per language. Cannot include price/promotion keywords ("free", "discount", "sale", "best", "#1", etc.) — Play Console will block promotion of the listing.** Live Play Store currently has "Snap, speak, or type a meal. AI logs the calories. Free & open source." which triggers the warning; replacement below drops "Free" while keeping the same rhythm. English-only on Play Console — non-English Play Store browsers see the English source as fallback.

### English (en-US) — 63 chars
```
Snap, speak, or type a meal. AI logs the calories. Open source.
```

---

## 3. Full Description

**4000 char hard cap per language.** This is the long-form "About this app" copy. English-only on Play Console — non-English Play Store browsers see the English source as fallback (deliberate decision; the in-app UI is fully translated via per-locale `values-{lang}/strings.xml` so users still get a localized experience once installed).

### English (en-US)
```
Fud AI makes calorie tracking effortless with AI-powered food recognition. Snap a photo, speak it, or type it — get instant nutrition: calories, protein, carbs, fats, and 9 micronutrients.

NEW in v1.0.11: Fud AI Plus is now on Android for no-key Gemini food scans, voice, and Coach. Bring Your Own Key remains available by default, and existing users get a one-time option to try Plus or keep BYOK.

Free, open source, privacy-first. Bring your own API key, or choose optional Fud AI Plus for no-key setup. Your food log stays on your device.

HOW TO USE
1) Set up your profile with goals + body stats
2) Snap, speak, type, or manually enter a meal — review and save
3) Ask Coach anything: trends, predictions, advice
4) Track progress on charts and home screen widgets

4 WAYS TO LOG A MEAL
• Photo — AI identifies the food and returns nutrition
• Voice — 5 STT engines with per-provider language selection
• Text — describe in plain language, AI parses it
• Manual Entry — name + calories + macros + meal type, no AI needed

BODY COMPOSITION TRACKING
Log body fat % over time, set a goal %, see it graphed alongside weight on the unified Progress chart. Health Connect sync auto-imports samples from Withings, Renpho, Samsung Health, Google Fit. "Use Body Fat for BMR" toggles Katch-McArdle ↔ Mifflin-St Jeor without losing the value.

13 AI PROVIDERS
Google Gemini, OpenAI, Anthropic Claude, xAI Grok, Groq, OpenRouter, Together AI, Hugging Face, Fireworks AI, DeepInfra, Mistral, Ollama (local), or any OpenAI-compatible endpoint. Switch anytime. OpenRouter defaults to a free vision model — test without loading credits. Keys stored encrypted (AES-256). Add Custom AI Instructions to send region, diet, or brand context with every request. Set a Fallback Provider so the app auto-retries on overload or rate-limit errors.

5 SPEECH-TO-TEXT ENGINES
Native Android, OpenAI Whisper, Groq, Deepgram, AssemblyAI. Choose Provider Auto, Use Device Language, or a fixed language.

COACH (TOOL CALLING)
Multi-turn chat that sees your profile, weight, body fat, and food log. Ask "what was my weight in March?" or "how's my protein this week?" — Coach pulls the date range it needs via 5 on-demand tools. It now understands today's date/timezone and richer meal details. Goal-aware chips for Lose / Gain / Maintain.

SMART DAILY REMINDERS
Log Weight, Log Body Fat, Streak, Daily Summary — all skip firing on days you've already logged, so fully-tracking users get effectively zero pings.

PERSONALIZED GOALS
BMR via Katch-McArdle (with body fat) or Mifflin-St Jeor. TDEE with 6 activity levels. Auto-calculated calorie + protein + carbs + fat targets — fully customizable.

PROGRESS
Unified Weight / Body Fat chart with trend lines + goal overlays. Calorie trend vs goal. Macro averages over 1W, 1M, 3M, 6M, 1Y, All Time.

WIDGETS
Calorie widget (pink-gradient ring with today's calories + macros) and Protein widget — both in Small 2x2 and Medium 4x2, refresh the moment you log a meal.

SAVED MEALS + SEARCH
Recents, Frequent, and Favorites tabs. Search bar filters each tab separately — substring, case-insensitive, diacritic-insensitive.

15 LANGUAGES
Auto-selected by phone language: English, Spanish, French, German, Italian, Portuguese (BR), Dutch, Russian, Japanese, Korean, Chinese, Hindi, Arabic, Romanian, Azerbaijani.

PRIVACY FIRST
No account, no sign-in, no cloud sync, no analytics, no ads, no tracking. Local-only. MIT licensed.

HEALTH CONNECT
Two-way sync for nutrition, weight, body fat. Macros + 9 micronutrients per meal. Edits and deletes sync back.

Built solo because tracking calories shouldn't feel like a chore. Reach out at apoorv@fud-ai.app, GitHub, or Instagram @fudai.app.

NOTE: Not medical advice. All nutritional estimates are AI-generated. Consult a healthcare professional before significant diet changes.

Terms: https://fud-ai.app/terms.html
Privacy: https://fud-ai.app/privacy.html
Source: https://github.com/apoorvdarshan/fud-ai
```

### Other 14 languages
English-only on Play Console — non-English Play Store browsers (ar, az-AZ, de-DE, es-ES, fr-FR, hi-IN, it-IT, ja-JP, ko-KR, nl-NL, pt-BR, ro, ru-RU, zh-CN) see the English source as fallback. The in-app UI itself is fully translated into all 14 locales via per-locale `values-{lang}/strings.xml`, so the localization gap is only on the Play Store listing surface, not inside the app.

---

## 4. What's New (v1.0.11)

**500 char hard cap per language.** Paste the entire block below into Play Console's "Release notes" field — it auto-routes each `<lang-tag>` block to the matching locale.

```
<en-US>
• Fud AI Plus is now on Android: no-key Gemini food scans, voice, and Coach.
• BYOK stays available by default, with a one-time Plus intro for existing users.
• Added Plus usage counters, restore, and Settings controls.
</en-US>

<ar>
• أصبح Fud AI Plus متاحًا على Android لمسح الطعام والصوت والمدرب بدون مفتاح API.
• يبقى BYOK متاحًا افتراضيًا، مع تعريف Plus مرة واحدة للمستخدمين الحاليين.
• تمت إضافة عدادات استخدام Plus والاستعادة والتحكم من الإعدادات.
</ar>

<az-AZ>
• Fud AI Plus Android-də açarsız Gemini qida skanı, səs və Coach üçün gəldi.
• BYOK defolt olaraq qalır, mövcud istifadəçilərə Plus bir dəfə göstərilir.
• Plus istifadə sayğacları, bərpa və ayar idarələri əlavə edildi.
</az-AZ>

<de-DE>
• Fud AI Plus ist jetzt auf Android: Gemini ohne API-Key für Food-Scans, Sprache und Coach.
• BYOK bleibt standardmäßig verfügbar, mit einmaligem Plus-Hinweis für bestehende Nutzer.
• Plus-Nutzung, Wiederherstellen und Einstellungen wurden ergänzt.
</de-DE>

<es-ES>
• Fud AI Plus llega a Android: Gemini sin clave para comida, voz y Coach.
• BYOK sigue disponible por defecto, con aviso único de Plus para usuarios existentes.
• Añadidos contadores de uso, restauración y controles de Plus.
</es-ES>

<fr-FR>
• Fud AI Plus arrive sur Android : Gemini sans clé pour repas, voix et Coach.
• BYOK reste disponible par défaut, avec une intro Plus unique pour les utilisateurs existants.
• Ajout des compteurs d'utilisation, restauration et contrôles Plus.
</fr-FR>

<hi-IN>
• Fud AI Plus अब Android पर है: बिना API key Gemini food scan, voice और Coach.
• BYOK default रहेगा, existing users को Plus का one-time intro मिलेगा.
• Plus usage counters, restore और Settings controls जोड़े गए.
</hi-IN>

<it-IT>
• Fud AI Plus arriva su Android: Gemini senza chiave per cibo, voce e Coach.
• BYOK resta disponibile di default, con intro Plus una sola volta per gli utenti esistenti.
• Aggiunti contatori uso Plus, ripristino e controlli in Impostazioni.
</it-IT>

<ja-JP>
• Fud AI Plus が Android に対応し、APIキーなしで Gemini の食事解析・音声・Coach が使えます。
• BYOK は引き続き標準で利用でき、既存ユーザーには Plus の案内を一度だけ表示します。
• Plus の使用量、復元、設定コントロールを追加しました。
</ja-JP>

<ko-KR>
• Fud AI Plus가 Android에 추가되어 API 키 없이 Gemini 음식 분석, 음성, Coach를 사용할 수 있습니다.
• BYOK는 기본으로 유지되며 기존 사용자에게 Plus 안내를 한 번 표시합니다.
• Plus 사용량, 복원, 설정 제어를 추가했습니다.
</ko-KR>

<nl-NL>
• Fud AI Plus is nu op Android: Gemini zonder API-key voor eten, spraak en Coach.
• BYOK blijft standaard beschikbaar, met een eenmalige Plus-intro voor bestaande gebruikers.
• Plus-gebruik, herstellen en instellingen toegevoegd.
</nl-NL>

<pt-BR>
• Fud AI Plus chegou ao Android: Gemini sem chave para comida, voz e Coach.
• BYOK continua disponível por padrão, com aviso único de Plus para usuários atuais.
• Adicionados contadores de uso, restauração e controles do Plus.
</pt-BR>

<ro>
• Fud AI Plus este acum pe Android: Gemini fără cheie pentru mâncare, voce și Coach.
• BYOK rămâne disponibil implicit, cu o introducere Plus unică pentru utilizatorii existenți.
• Am adăugat contoare de utilizare, restaurare și controale Plus.
</ro>

<ru-RU>
• Fud AI Plus теперь на Android: Gemini без API-ключа для еды, голоса и Coach.
• BYOK остается доступным по умолчанию, с одноразовым знакомством с Plus для текущих пользователей.
• Добавлены счетчики Plus, восстановление и настройки.
</ru-RU>

<zh-CN>
• Fud AI Plus 已支持 Android：无需 API key 即可使用 Gemini 食物扫描、语音和 Coach。
• BYOK 仍默认可用，现有用户会看到一次 Plus 介绍。
• 新增 Plus 用量计数、恢复购买和设置控制。
</zh-CN>
```

---

## 5. Categorization

```
App category: Health & Fitness
Tags: Calorie tracker, Nutrition, AI, Food tracker
```

## 6. Contact details

```
Email: apoorv@fud-ai.app
Phone: (omit — optional, US-only enforcement)
Website: https://fud-ai.app
Privacy policy: https://fud-ai.app/privacy.html
```

## 7. App content declarations

These are one-time setup in Play Console → Policy → App content. Don't drift from these answers across submissions:

- **Privacy policy URL**: https://fud-ai.app/privacy.html
- **App access**: All functionality available without restrictions
- **Ads**: No
- **Content rating**: Everyone (E)
- **Target audience**: 13+
- **News app**: No
- **COVID-19 contact tracing**: No
- **Data safety**: All processing on-device. No data collected/shared. API keys stored in EncryptedSharedPreferences. Encryption in transit when calling AI provider APIs (HTTPS). User can request deletion via in-app "Delete All Data" — no server data exists.
- **Government app**: No
- **Financial features**: No
- **Health features**: Yes — fitness/nutrition tracking. Local-only.
