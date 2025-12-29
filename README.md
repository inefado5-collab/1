//simpan di setting.js

global.owner = ["6281572480595"];
global.developer = [
    "628xxxxxxxxx", // contoh: nomor kamu
    "62813xxxxxxx"
];
global.botname = "Theresa";
global.website = "https://theresapis.vercel.app";
global.ownername = "Z7:林企业";
global.footer = `♡₊˚ I am Theresa ˚₊♡`;
global.defaultLimit = 100;
global.idch = "120363420385250482@newsletter";
global.fgsi = "fgsiapi-292d345-6d";
global.botnumber = "6285123675946";
//TEMPAT APIKEY
global.betaAiKey = "THERESA";
global.alyachan = "https://api.alyachan.dev";
global.tokengh = "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";
global.googleAiApiKey = "AIzaSyCDzhosCdX1F3PgwJW3jzubU37DX5xD2lU";
//THUMBAIL
global.thumb =
    "https://raw.githubusercontent.com/belluptaka/dat3/main/uploads/38a0cd-1764738729608.jpg";
global.menuVn = "https://files.catbox.moe/4hgknq.mp3";
global.linkch = "https://whatsapp.com/channel/0029VbBt4432f3ENa8ULoM1J";
global.loading = (m, conn, back = false) => {
    if (!back) {
        return conn.sendReact(m.chat, "🕒", m.key);
    } else {
        return conn.sendReact(m.chat, "", m.key);
    }
};

global.isDeveloper = jid => {
    if (!jid) return false;
    const num = jid.replace(/[^0-9]/g, "");
    return global.developer.includes(num);
};

//simpan di index.js

ini tempalkan di bawah ini

(global.db = db;
global.interactiveSessions = new Map(); // Untuk fitur pesan interaktif
global.displayedBanner = false;)

terus ini tempel kan 👇

global.isDeveloper = (jid) => {
    if (!jid) return false;
    const num = jid.replace(/[^0-9]/g, "");
    return Array.isArray(global.config?.developer)
        ? global.config.developer.includes(num)
        : false;
};

// simpan di handler.js

  const sender = fixJid(decodeJid(m.sender || m.jid));
simpan di atas ini 👆

yang di ambil di bawah ini 👇

  const isdeveloper = global.isDeveloper(sender);

  // masih di handler.js

  ini simpan di bawah register

  if (handler.developer && !isdeveloper) {
                m.reply("perintah ini hanya bisa di gunakan oleh developer");
                continue;
            }
