# AI Hub — barcha AI vositalari va konektorlar bir joyda

Bu papka Claude (cloud) ga ulangan barcha AI vositalari, konektorlar va ularning sozlamalari ro'yxatini saqlaydi. Keyingi ishlar shu repo orqali olib boriladi.

> ⚠️ **Repo PUBLIC (ochiq).** Bu yerga hech qachon API kalit, token, parol yoki shaxsiy e-mail yozilmaydi. Kalitlar faqat kompyuterdagi lokal konfiguratsiyada yoki `.env` faylida turadi (`.env` git'ga tushmaydi — `.gitignore` ga qarang).

## Tuzilma

| Papka | Nima bor |
|---|---|
| [`connectors/`](connectors/README.md) | Cloud konektorlar: Google Drive, Notion, Windsor.ai, Zapier |
| [`local-mcp/`](local-mcp/README.md) | Kompyuterdagi lokal MCP serverlar: Gemini, UzbekVoice (+ konfiguratsiya shabloni) |
| [`skills/`](skills/README.md) | Claude'dagi yoqilgan skill'lar ro'yxati |
| `inventory.json` | Hammasining mashina o'qiy oladigan ro'yxati |

## Holat (2026-11-18)

| Vosita | Turi | Holat |
|---|---|---|
| Google Drive | Cloud konektor | ✅ ulangan |
| Notion | Cloud konektor | ✅ ulangan |
| Windsor.ai | Cloud konektor | ✅ ulangan (Instagram, YouTube) |
| Zapier | Cloud konektor | ✅ ulangan (YouTube) |
| Gemini | Lokal MCP (Windows) | ✅ ishlayapti |
| UzbekVoice | Lokal MCP (Windows) | ⚠️ kalit bor, lekin server HTTP 404 qaytaryapti — tekshirish kerak |

## Muhim eslatma

Cloud konektorlarning o'zi (OAuth ulanishlar) GitHub'ga ko'chirilmaydi — ular claude.ai hisobida turadi va **Settings → Connectors** orqali boshqariladi. Bu repoda ularning ro'yxati, imkoniyatlari va ish tartibi saqlanadi, Claude esa har bir sessiyada shu yerdan ma'lumot olib ishlaydi.

## Yangi vosita qo'shish

1. Tegishli papkaga `.md` fayl qo'shing (namunaga qarab).
2. `inventory.json` ga yozuv qo'shing.
3. Maxfiy kalitlarni **yozmang** — faqat o'zgaruvchi nomini (`GEMINI_API_KEY` kabi) ko'rsating.
