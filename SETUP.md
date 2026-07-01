# ברוש Telegram Bot — מדריך התקנה (5 דקות)

## שלב 1 — צור בוט ב-Telegram (2 דקות)

1. פתח Telegram וחפש: **@BotFather**
2. שלח: `/newbot`
3. תן שם לבוט: `ברוש AI` (או כל שם)
4. תן username: `BroshAI_bot` (חייב להסתיים ב-bot)
5. תקבל **Token** — שמור אותו! נראה כך:
   `7234567890:AAFxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`

---

## שלב 2 — הכן את הקבצים

```bash
# פתח את תיקיית הפרויקט
cd brosh-telegram-bot

# התקן תלויות
npm install

# צור קובץ .env
echo "TELEGRAM_BOT_TOKEN=TOKEN_שלך_כאן" > .env
echo "ANTHROPIC_API_KEY=sk-ant-xxxxx" >> .env
```

---

## שלב 3 — הרץ (Railway — חינמי)

**אפשרות א׳ — Railway (מומלץ, חינמי):**
1. כנס ל-[railway.app](https://railway.app) והתחבר עם GitHub
2. New Project → Deploy from GitHub → בחר את הריפו
3. הוסף Variables:
   - `TELEGRAM_BOT_TOKEN` = הtoken מ-BotFather
   - `ANTHROPIC_API_KEY` = המפתח שלך
4. Deploy — הבוט עולה תוך דקה

**אפשרות ב׳ — הרצה מקומית לבדיקה:**
```bash
npm run dev
```

---

## שלב 4 — הוסף לקבוצה

1. צור קבוצת Telegram: "ברוש AI 🏢"
2. הוסף את הבוט לקבוצה (חפש לפי username)
3. שלח `/start` בקבוצה
4. כל אחד בקבוצה יכול לשאול שאלות!

---

## פקודות הבוט

| פקודה | תיאור |
|---|---|
| `/start` | פתיחה וברכה |
| `/help` | דוגמאות לשאלות |
| `/reset` | איפוס זיכרון השיחה |

---

## דוגמאות לשימוש

> מה שטח דירה 15 ביהודה המכבי?
> מי האדריכל של פישמן מימון 16?
> כמה יחידות יזם יש בביאליק 36?
> מה הטלפון של קרן ברק?
> סטטוס מכירות לואי מרשל

---

## עלות: חינמי לחלוטין 🎉
- Telegram API: חינמי
- Railway: חינמי (500 שעות/חודש — מספיק)
- Anthropic API: ~$5-10/חודש לשימוש פנימי
