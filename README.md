# HR Notion Bot

Notion databasedagi yangi anketalarni Telegram ga yuboradi.

## Ishlash prinsipi
- Har 60 soniyada Notion DB ni tekshiradi
- `Yuborildi = False` bo'lgan yozuvlarni topadi
- Telegram ga yuboradi
- `Yuborildi = True` qilib belgilaydi

## Notion Database da kerakli ustunlar

| Ustun nomi | Turi |
|---|---|
| ФИШ | Title |
| Lavozim | Text |
| Telefon | Phone |
| PINFL | Text |
| Ish boshlagan sana | Date |
| Maosh istagi | Number |
| Yuborildi | Checkbox |

## Railway da deploy

1. GitHub repo ni Railway ga ulang
2. Environment variables qo'shing (`.env.example` ga qarang)
3. Deploy

## Environment Variables

```
NOTION_TOKEN=secret_xxx
NOTION_DB_ID=xxx
TELEGRAM_TOKEN=xxx
TELEGRAM_CHAT_ID=@kanal_yoki_chat_id
```
