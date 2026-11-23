# DYOR Coin Observatory

## О проекте / токене

Согласно метаданным контракта, DYOR Coin — служебный токен аналитической платформы DYOR.io.

Самоописание из метаданных токена; заявления проекта не проверены независимо.

Источники (проверены 2026-11-23):

- <https://tonapi.io/v2/jettons/EQCQZpelevHNsbw5IUtwSa4Cs8kqWww0KsYeDri9kwS18eCz>

Generated from https://github.com/Freebielife/TON-Observatory-Template.

Run python3 -m scripts.refresh_observatory; python3 build.py; python3 verify.py.
Publish index.html in TON Sites only after independent on-chain verification.
Собран первый проверенный снимок данных DYOR. История сделок пополняется постепенно; наличие переключателя «Год» не означает полный год данных.
Only native TON swap pairs supported. Locks, staking and custom project NFT badges are configured through project.json and verified against TonAPI.
Workflow update.yml подготовлен для ручного запуска и внешнего планировщика. Подключение к действующему Cloudflare-планировщику и фактический интервал 30 минут пока не подтверждены.

Foundation version: 1.3.0. Holders show 10, expandable to top 20.
`project.json` is the per-project specification. Contract/pool/precision changes require regenerating from the factory; do not reuse another token's snapshot.
Run `python3 build.py` for an atomic bundle and `build/report.json` size report.
No external fonts, scripts or images are needed to render the saved page. Fresh data checks and manual wallet lookups require network access.
Cloudflare dispatch registration and GitHub repository access remain separate deployment steps. No credentials go into HTML.

## Брендинг и проверки

- Точность DYOR: 15; точность TON: 9.
- Логотип: изображение, предоставленное владельцем 2026-11-23; официальный источник указан в project.json.
- Флаг: TONecoFlags №095 из предоставленного каталога.
- Каналы: https://t.me/DYORNinja и https://t.me/DYORNinjaRU.
- Проверены мобильная ширина 390 px, отсутствие горизонтального переполнения, RU/EN, TON/USD, раскрытие 10 → 20 холдеров и встроенные ресурсы.
- Заморозка и стейкинг не подключены; отсутствующие сведения не заменяются нулями.
- Публикация в TON Storage / Resistance Tools в рамках этой сборки не выполнена.

Текущий снимок: 223 сделок; незавершённые разделы: fragmentNumbers. Проверки: 17 Python, 15 Node; HTML и токен проверены. Публикация main ожидает отдельного разрешения.
