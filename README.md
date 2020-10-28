const Discord = require("discord.js");
const client = new Discord.Client();
const ayarlar = require("./ayarlar.json");

const Eserver = new Discord.WebHookClient(
  "770994976842448947",
  "bsG-DIKSPoN9jAt4-_qWfhNkbARuIebFxgIcbzuiWlk8WN0otXuVDXV5eDvYDbSH6-8L"
); //hosgeldin mesajı

client.on("guildMemberAdd", member => {
  Eserver.send(`${member} Hoşgeldin onii-chan.`);
});
