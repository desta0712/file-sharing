{
  "name": "File Sharing Superman",
  "description": "BOT Multi Force Subs File Sharing Bot berguna untuk menyimpan file dan dapat diakses melalui link khusus",
  "keywords": [
    "telegram",
    "file",
    "sharing"
  ],
  "repository": "https://github.com/Stinkyrz/Stinky-Filesharing",
  "logo": "https://telegra.ph/file/2c5ec091fb6e96628e610.jpg",
  "env": {
    "TG_BOT_TOKEN": {
      "description": "Masukan Bot token, Dapatkan dari t.me/BotFather",
      "value": ""
    },
    "OWNER": {
      "description": "Masukan Username Telegram untuk Owner BOT [ Jangan Pake @ ]",
      "value": "Callme_stinky"
    },
    "OWNER_ID": {
      "description": "Masukan User ID Telegram untuk Owner BOT",
      "value": "1435206452"
    },
    "APP_ID": {
      "description": "Dapatkan APP ID di web my.telegram.org",
      "value": ""
    },
    "API_HASH": {
      "description": "Dapatkan API HASH di web my.telegram.org",
      "value": ""
    },
    "CHANNEL_ID": {
      "description": "Masukan ID Channel Untuk [Channel Database]",
      "value": "-100"
    },
    "FORCE_SUB_CHANNEL": {
      "description": "Masukan ID dari Channel Atau Group Untuk Wajib Subscribenya",
      "value": "-100"
    },
    "FORCE_SUB_GROUP": {
      "description": "Masukan ID dari Group Untuk Wajib Subscribenya",
      "value": "-100"
    },
    "START_MESSAGE": {
      "description": "Pesan /start memulai awalan ke bot, Gunakan format parsemode HTML",
      "value": "<b>Hello {first}\n\nJika mau repo file sharing seperti ini bisa cek disini @Stinkyrz owner repo @Callme_stinky.</b>"
    },
    "FORCE_SUB_MESSAGE": {
      "description": "Pesan Paksa Subscribe bot, Gunakan Format parsemode HTML",
      "value": "<b>Hello {first}\n\nAnda harus bergabung di Channel/Grup saya untuk menggunakan saya\n\nSilakan Join Ke Channel Terlebih Dahulu</b>"
    },
    "CHANNEL":{
      "description": "Masukan Username Channel anda Untuk Wajib Subscribenya [ Jangan Pake @ ]",
      "value": "Stinkyrz",
      "required": false
    },
    "GROUP":{
      "description": "Masukan Username dari Group anda Untuk Wajib Subscribenya [ Jangan Pake @ ]",
      "value": "PHS_ID",
      "required": false
    },
    "ADMINS": {
      "description": "Masukan User ID untuk mendapatkan hak Admin BOT [Hanya dapat membuat link]",
      "value": "",
      "required": false
    }
  },
  "addons": [
    {
    "plan": "heroku-postgresql",
      "options": {
        "version": "12"
      }
    }
  ],
  "buildpacks": [
    {
      "url": "heroku/python"
    }
  ],
  "formation": {
    "worker": {
      "quantity": 1,
      "size": "free"
    }
  }
}
