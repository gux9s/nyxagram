<p align="center">
  <img src="https://raw.githubusercontent.com/yozuxo/nyxagram/main/.github/logo.png" width="112" alt="Nyxagram">
</p>

<h1 align="center">Nyxagram</h1>

<p align="center"><b>Unofficial Telegram client for iPhone</b><br>more control over what others see, and a few tools Telegram doesn't have</p>

<p align="center">
  <a href="https://github.com/yozuxo/nyxagram/releases/latest/download/Nyxagram.ipa"><img src="https://img.shields.io/badge/Download-Nyxagram.ipa-black?style=for-the-badge&logo=apple&logoColor=white" alt="Download"></a>
</p>

<p align="center">
  <a href="https://github.com/yozuxo/nyxagram/releases/latest"><img src="https://img.shields.io/github/v/release/yozuxo/nyxagram?style=flat-square&color=black&label=version" alt="Version"></a>
  <img src="https://img.shields.io/badge/iOS-15%2B-black?style=flat-square" alt="iOS 15+">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-GPL--2.0-blue?style=flat-square" alt="GPL-2.0"></a>
  <a href="https://t.me/nyxagram"><img src="https://img.shields.io/badge/Telegram-@nyxagram-2CA5E0?style=flat-square&logo=telegram&logoColor=white" alt="Telegram"></a>
</p>

> **Nyxagram is not the official Telegram app and is not affiliated with Telegram in any way. Please don't confuse the two.** It uses the Telegram API and is built from the open Telegram-iOS source.

---

## Features

### Privacy
- **Ghost mode**: hide read receipts, online status, typing, story views and voice message plays
- **Deleted messages stay**: yours and the other person's, marked in the chat
- **Face ID lock** for chosen chats
- Hide your phone number, the stories bar and message text in the chat list

### Chat
- **Edit history**: see what a message said before it was changed
- **Autocorrect**: typos, spaces, capitals and the most obvious commas, fixed on the device when you send
- **Translator** on the device (iOS 18+), no Telegram Premium needed
- Time with seconds, silent sending by default, confirm calls and stickers, review voice messages before they go

### Profile
- Streaks, previous names and usernames, ID, data center and registration date
- Avatar frames and a video background for your profile
- Device name spoofing in your sessions list

### Local only (visible just to you, on this device)
- Fake gifts, stars and Gram, with upgrade, pin and purchase history
- Fake usernames and phone number, fake level, local Premium

### Tools
- **Find by ID**: open a profile or chat by its numeric ID
- **Backup**: all settings in one file

Everything is in **Settings → Nyxagram**.

## Install

1. Download [`Nyxagram.ipa`](https://github.com/yozuxo/nyxagram/releases/latest/download/Nyxagram.ipa)
2. Sign and install it with any sideloading app, for example ESign, Scarlet or Sideloadly

## Source

`nyxa.patch` goes on top of [Telegram-iOS](https://github.com/TelegramMessenger/Telegram-iOS) at the commit in `UPSTREAM_COMMIT`:

```sh
git clone --recursive https://github.com/TelegramMessenger/Telegram-iOS.git
cd Telegram-iOS
git checkout "$(cat ../UPSTREAM_COMMIT)"
git apply ../nyxa.patch
```

then build it as described in the Telegram-iOS README, with your own `api_id` and `api_hash`.

## License

GPL-2.0, like Telegram-iOS. This is a modified version of it, and all the changes are in `nyxa.patch`.

<details>
<summary><b>По-русски</b></summary>

**Nyxagram** — неофициальный клиент Telegram для iPhone. Он не связан с Telegram, не путайте их.

**Возможности**
- **Приватность:** режим призрака (прочтение, «в сети», «печатает», истории, голосовые), сохранение удалённых сообщений, Face ID на чатах
- **Чат:** история изменений, автоисправление при отправке, переводчик на устройстве (iOS 18+) без Premium, время с секундами, тихая отправка
- **Профиль:** огонёк, прежние имена, ID и дата регистрации, рамки и видеофон, подмена названия устройства
- **Только у вас на устройстве:** fake подарки, звёзды и Gram, юзы, номер, уровень, локальный Premium
- **Инструменты:** поиск по ID, бэкап настроек одним файлом

Всё в **Настройки → Nyxagram**.

**Установка:** скачайте [`Nyxagram.ipa`](https://github.com/yozuxo/nyxagram/releases/latest/download/Nyxagram.ipa) и поставьте через ESign, Scarlet или Sideloadly.

**Исходники:** `nyxa.patch` накладывается на Telegram-iOS по коммиту из `UPSTREAM_COMMIT`. Лицензия GPL-2.0.

</details>
