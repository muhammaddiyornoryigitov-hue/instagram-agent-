# Cloud konektorlar

Bular claude.ai hisobiga ulangan va Claude'ning har bir sessiyasida mavjud. Ulash/uzish: **claude.ai → Settings → Connectors**.

## Google Drive
- **Vazifa:** fayllarni qidirish, o'qish, yaratish, yangilash, ulashish.
- **Asosiy amallar:** `search_files`, `read_file_content`, `create_file`, `update_file`, `copy_file`, `share_file`, `trash_file`, `list_recent_files`.

## Notion
- **Vazifa:** sahifalar, bazalar, kalendar, izohlar, uchrashuv qaydlari.
- **Asosiy amallar:** `notion-search`, `notion-fetch`, `notion-create-pages`, `notion-update-page`, `notion-query-data-sources`, `notion-calendar-*`, `notion-create-comment`.

## Windsor.ai
- **Vazifa:** 350+ manbadan analitika o'qish va ijtimoiy tarmoqlarga yozish.
- **Ulangan akkauntlar:**
  - **Instagram** — `@hafsa_ustoza`
    - Yozish amallari: `create_video_post`, `create_image_post`, `create_carousel_post`, `create_story`, `create_comment`, `reply_to_comment`, `delete_comment`, `hide_comment`, `unhide_comment`
  - **YouTube** — Hafsa ustoza kanali
    - Yozish amallari: `update_video_details`, `add_video_to_playlist`, `remove_video_from_playlist`, `reply_to_comment`, `moderate_comment`, `delete_comment`
- **Eslatma:** yozish amallari faqat foydalanuvchi aniq tasdiqlagandan keyin bajariladi.

## Zapier
- **Vazifa:** 9000+ ilova bilan avtomatlashtirish.
- **Yoqilgan ilovalar:** YouTube (12 ta amal, 1 ta ulanish).
- **Zapier skill'lari:** `onboarding`, `mcp-roast` (o'rnatilgan).
- Yangi ilova qo'shish: Claude'ga "Zapier'ga <ilova> qo'sh" deb yozing.

## Instagram video yuklash oqimi (shu repo bilan)
1. Video shu reponing `media` branch'iga vaqtincha yuklanadi.
2. Windsor.ai `create_video_post` orqali Instagram'ga joylanadi (raw GitHub havolasi orqali).
3. Joylangandan keyin video repodan o'chiriladi.
