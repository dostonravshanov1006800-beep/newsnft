# Newsnft — Premium NFT Gifts

Telegram Mini App: апгрейд подарков, маркет с floor-ценами, крафт, инвентарь.
Архитектура: чистый GitHub, без серверного кода (как gift-rental-bot).

- **Frontend**: GitHub Pages, один статический index.html
- **Данные**: data/*.json через raw.githubusercontent.com (обновляет Actions-бот)
- **Бот**: GitHub Actions keep-alive (публичный репо = неограниченные бесплатные минуты)
- **TON Connect 2**: манифест — статика tonconnect-manifest.json (кошелёк для отображения)

## Roadmap
- [x] Статический апп на Pages, чужие бэкенды вырезаны
- [ ] Actions-бот: floor-цены (api.changes.tg) -> data/floors.json
- [ ] Инвентарь: getUserGifts-скан -> data/gifts/<uid>.json
- [ ] Честные спины: результат считает бот (провably-fair SHA-256), баланс в data/balance/<uid>.json
