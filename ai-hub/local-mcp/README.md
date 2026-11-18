# Lokal MCP serverlar (Windows kompyuter)

Bu serverlar Claude desktop ilovasi orqali kompyuterda ishlaydi. Claude cloud sessiyasi ularga desktop ilova ochiq va onlayn bo'lgandagina ulanadi.

Konfiguratsiya fayli: `%APPDATA%\Claude\claude_desktop_config.json`
Shablon: [`claude_desktop_config.example.json`](claude_desktop_config.example.json) — haqiqiy kalitlar o'rniga `<...>` yozilgan.

## Gemini
- **Vazifa:** Google Gemini modellari bilan ishlash.
- **Amallar:** `ask_gemini`, `search_with_gemini`, `analyze_file`, `generate_image`, `list_gemini_models`.
- **Kalit:** `GEMINI_API_KEY` (faqat lokal konfiguratsiyada).
- **Mavjud modellar (2026-11-18):** gemini-2.5-flash, gemini-2.5-pro, gemini-3.5-flash, gemini-3.6-flash, gemini-3.7-flash, gemini-3.8-flash, gemini-3-pro-image, gemini-3.1-flash-image, gemini-nano-banana-2.1, gemini-4-argon/carbon/hydrogen, gemma-4-31b-it, deep-research-* va boshqalar.

## UzbekVoice
- **Vazifa:** o'zbek tilida matn → ovoz (TTS) va ovoz → matn (STT).
- **Amallar:** `uzbekvoice_tts`, `uzbekvoice_stt`, `uzbekvoice_list_audio`, `uzbekvoice_check`.
- **Kalit:** `UZBEKVOICE_API_KEY` (faqat lokal konfiguratsiyada).
- **Natijalar papkasi:** `~/UzbekVoice/Claude outputs`
- ⚠️ **Holat:** kalit topildi, lekin server `HTTP 404` qaytardi — API manzili yoki kalit muddatini tekshirish kerak.

## Server kodini shu repoga qo'shish
Serverlarning manba kodi (`.js` / `.py`) kompyuterda turadi. Uni bu yerga ko'chirish uchun Claude'ga papkaga ruxsat bering — kod kalitlarsiz ko'chiriladi.
