const express = require('express');

const app = express();

app.get('/', (req, res) => {
  res.send('Hello Express app!')
});

app.listen(3000, () => {
  console.log('server started');
});

const Discord = require("discord.js");
const client = new Discord.Client();
const prefix = "s!"
client.login("ODQzOTIxNTI0MTUwNjMyNDcw.YKK5Kg.nwbCczgzVlpokShwGS1vRT9k-ro")

///جميع الحقوق محفوضة لZakaria🍁#4675
 const figlet = require ("figlet");

client.on('message', saif => {
if (saif.content.startsWith(prefix + 'tag')) {
    let args = saif.content.split(" ").slice(1);
if(!args[0]) return saif.reply('i dont see any word !?!');  

    figlet(args.join(" "), (err, shark) => {
              saif.channel.send(`\`\`\`${shark}\`\`\``)
           })
}
});

///جميع الحقوق محفوضة لZakaria🍁#4675
client.on('message', message => {
  var args = message.content.split(/[ ]+/)
  if(message.content.includes('discord.gg')){
    if(!message.member.hasPermission('ADMINISTRATOR'))
      message.delete()
  return message.reply(`** No Invite Links :angry: ! **`)
  }
});


///جميع الحقوق محفوضة لZakaria🍁#4675

client.on('message', badboy => {
  if(badboy.content.startsWith(prefix + "die")){
    let args = badboy.content.split(" ").slice(1).join(" ")
    if(!args) return badboy.reply("Please Mention Someone.")
let user = badboy.mentions.users.first();user.username

      if (user.id == badboy.author.id) return badboy.reply("You cannot use this command with yourself.")

if(badboy.author.bot || !badboy.guild) return badboy.reply("this command for server only")
let die = [
 "https://media.tenor.com/images/751d6257579f90047c3eed57a642dd1c/tenor.gif"
  ];
 
    
    
    let embed = new Discord.MessageEmbed()
    .setTitle(`${badboy.author.username}:skull: :skull_and_crossbones: ${user.username}  `)
    .setImage(`${die}`)
    
    .setFooter(`Requsted by ${badboy.author.username}`)
badboy.channel.send(embed)
  
  }
})

///جميع الحقوق محفوضة لZakaria🍁#4675
client.on('message', badboy => {
    if(badboy.content.startsWith(prefix + "hug")){
      
let user = badboy.mentions.users.first();user.username

if(!user) return badboy.reply("منشن الشخص")
      let hugs = [
        'https://cdn.discordapp.com/attachments/782532317729652757/797086131018924032/tenor.gif',
        

        ];
  let hug1 = hugs[Math.floor(Math.random() * hugs.length)];
  
  var embed = new Discord.MessageEmbed()
  .setTitle("HUG")
     .setImage(`${hug1}`)
.setFooter(`${badboy.author.username} has hug ${user.username}`)
      badboy.channel.send(embed)
   
    }
  })

  client.on('message', message => {
  if (message.content === (prefix + 'invite') || message.content === (prefix + 'inv')){
  var embed = new Discord.MessageEmbed()

.setTitle(`**Support**`)

.setDescription(`
.[Link added bot /رابط اضافت البوت](https://discord.com/api/oauth2/authorize?client_id=838588452533698570&permissions=8&scope=bot)


**شكرا على اختيارك بوتنا | Thank you for choosing our bot :rose:.**


**Support /سيرفر الدعم الفني
**
https://discord.gg/QPvHSEyCqq `)

.setFooter(`by  ⚜ 𝐂𝐀𝐙𝐀⚜  
Remake TPK salem`)

message.channel.send(embed);
  }
});

///جميع الحقوق محفوضة لZakaria🍁#4675
 
   client.on("message", jxa => {
    if (jxa.content === prefix + "server") {
  
  
      let embed = new Discord.MessageEmbed()
      .setTitle(`${jxa.guild.name}`)
      .setFooter(`Developer :  ⚜ 𝐂𝐀𝐙𝐀⚜ `)
        .setDescription(`**
   :id:   **ID Server** : ${jxa.guild.id}

   :crown: **Owner Server** : ${jxa.guild.owner}

  :globe_with_meridians:**Created** : ${jxa.guild.createdAt.toLocaleString()}

  :part_alternation_mark:  **Members** : ${jxa.guild.memberCount}

  :no_smoking: **Channels** : ${jxa.guild.channels.cache.size}
   
   :man_detective:  **Region** : ${jxa.guild.region}
    **`);
    jxa.channel.send(embed);
    }
  });

///جميع الحقوق محفوضة لZakaria🍁#4675
  client.on("message", msg => {
    if(msg.content === (prefix + 'help'))

    var embed = new Discord.MessageEmbed()
    .setFooter(`Developer :  𝕯𝖆𝖗𝖐 𝕬𝖓𝖌𝖊𝖑 `)
    .setColor("RANDOM")
    .setTitle(`\`\`${client.user.username}\`\` **help**`)
    .setDescription(`
  :beginner: **General Commands**

\`\`s!user,  s!server,

 s!ping, s!inv, s!say, s!tag\`\`

:beginner:  ** Admin Commands**

\`\`s!ban, s!اسكت, s!clear, s!lock, s!unlock,

 s!hide, s!show \`\`

:beginner:**Fun Commands**

\`\`s!cut,  s!die, s!hug s!spank, s!rip, s!Fruits,

 s!kill, s!trash, s!delete\`\`

`)
msg.channel.send(embed)
  });
client.on('message', badboy => {
  if(badboy.content.startsWith(prefix + "cut")){
    let cuts = [
      'ما هو لون هاتفك',
      'ما هو باسورد هاتفك',
      'هل تامن بلحب من اول نظرة؟',
      'كم مرا حبيت بنت',
      ' ._. هل تحب البطاطا',
           'اين تسكن',
                 'لو معاك مليون شن كنت حدير بيهن',
                            'شن حاجه يلي اول ما تشوفها تتريح ',
                                 'مكان تبي تمشيله ',
                                         ' اغلي حاجه شريتها ',
      
      ];
    
   let cut2 = cuts[Math.floor(Math.random() * cuts.length)];
var embed = new Discord.MessageEmbed()
.setTitle("Cut")
.setDescription(`${cut2}`)
.setThumbnail(`${badboy.author.avatarURL({dynamic : true})}`)
.setColor("BLUE")
    .setFooter(`Developer : ⚜ 𝐂𝐀𝐙𝐀⚜ `)

      badboy.channel.send(embed)
      
  }
})

///جميع الحقوق محفوضة لZakaria🍁#4675
client.on("message", jxa => {
    if(jxa.content === (prefix + 'ping'))
    var embed = new Discord.MessageEmbed()
    .setTitle(`\`\`${client.user.username}\`\` **Ping**<a:pp472:777667628528697404>`)
    .setDescription(`**My Ping Is**\`\`${client.ws.ping}\`\``)
    .setFooter(`Developer :  ⚜ 𝐂𝐀𝐙𝐀⚜ `)
   jxa.channel.send(embed)
  });


 
client.on('message', message=> {
    if (message.author.bot) return;
    if (message.mentions.has(client.user))
    {
    message.reply(`**My Prefix Is** : \`${prefix}\``)
    }
});


client.on('message', message => {
    let args = message.content.split(' ');
    if (message.content.startsWith(prefix + 'profile')) {
        let member = message.mentions.users.first();

        if (args[0] && !args[1]) {
            message.channel.startTyping();
            setTimeout(() => {
                message.channel.stopTyping();
            }, Math.random() * (1 - 3) + 1 * 1000);
            message.channel.send({
                files: [
                    {
                        name: 'https://probot.media/TKbe6YcB77.png',
                        attachment: `https://probot.media/TKbe6YcB77.png${message.author.id}`
                    }
                ]
            });
        }
        if (member) {
            message.channel.startTyping();
            setTimeout(() => {
                message.channel.stopTyping();
            }, Math.random() * (1 - 3) + 1 * 1000);
            message.channel.send({
                files: [
                    {
                        name: 'https://probot.media/TKbe6YcB77.png',
                        attachment: `https://probot.media/TKbe6YcB77.png${member.id}`
                    }
                ]
            });
        } else if (args[1] && !member) {
            client.users.fetch(args[1]).then(userr => {
                message.channel.stopTyping();
                setTimeout(() => {
                    message.channel.stopTyping();
                }, Math.random() * (1 - 3) + 1 * 1000);
                message.channel.send({
                    files: [
                        {
                            name: 'https://probot.media/TKbe6YcB77.png',
                            attachment: `https://probot.media/TKbe6YcB77.png${userr.id}`
                        }
                    ]
                });
            });
        }
    }
});

///جميع الحقوق محفوضة لZakaria🍁#4675
client.on("message",async message =>{
    let command = message.content.toLowerCase().split(" ")[0];
        command = command.slice(prefix.length);
    if (command == "clear" || command == "مسح") { 
    message.delete({timeout: 0})
        if(!message.channel.guild) return message.reply(`** This Command For Servers Only**`); 
         if(!message.member.hasPermission('MANAGE_GUILD')) return message.channel.send(`> ** You don't have perms :x:**`);
         if(!message.guild.member(client.user).hasPermission('MANAGE_GUILD')) return message.channel.send(`> ** I don't have perms :x:**`);
     
        let args = message.content.split(" ").slice(1)
        let messagecount = parseInt(args);
        if (args > 100) return message.channel.send(`\`\`\`javascript
    i cant delete more than 100 messages 
    \`\`\``).then(messages => messages.delete(5000))
    if(!messagecount) messagecount = '50';
        message.channel.messages.fetch({limit: 100 }).then(messages => message.channel.bulkDelete(messagecount)).then(msgs => {
        message.channel.send(`\`\`\`js
    ${msgs.size} messages cleared
    \`\`\``).then(messages => 
    messages.delete({timeout:5000}));
        })
      }    
    });
  
  client.on("message",message => {
    if(message.content.startsWith(prefix + "user")){
  let embed = new Discord.MessageEmbed()
  .setColor("RANDOM")
      .setFooter(`Developer : ⚜ 𝐂𝐀𝐙𝐀⚜ `)

  .setAuthor(message.author.username,message.author.avatarURL())
  .setThumbnail(message.author.avatarURL())
  .setTitle("Info User")
  .addField(':credit_card:``Name``', 
  ` ${message.author.tag} `, true)
  .addField(':id: ``ID``', 
  ` ${message.author.id} `, true)  
  .addField(':calendar_spiral: ``Created At``',
   ` ${message.author.createdAt.toLocaleString()} `, true)
  .setTimestamp(); 
  message.channel.send(embed)
  }
  });

  client.on('message', async message => {
if(message.content.startsWith(prefix + 'اسكت')) {
let mention = message.mentions.members.first();
let role = message.guild.roles.cache.find(ro => ro.name == 'Muted');
 
if (!message.guild.me.hasPermission('MANAGE_ROLES')) {
        const embed = new Discord.MessageEmbed()
.setThumbnail(client.user.avatarURL())
.setColor("RED")
.setTitle("Error ❌")
.setDescription("** انا لا امتلك برمشن المطلوب `MANAGE_ROLES` **")
.setFooter(client.user.username,client.user.avatarURL())
message.channel.send(embed);
};
if (!message.member.hasPermission('MANAGE_GUILD')) {
    const embed = new Discord.MessageEmbed()
.setThumbnail(client.user.avatarURL())
.setColor("RED")
.setTitle("Error ❌")
.setDescription(`**انت لا تمتلك البرمشن المطلوب MANAGE_GUILD**`)
    .setFooter(`Developer :  ⚜ 𝐂𝐀𝐙𝐀⚜ `)

};
 
let muteRole = message.guild.roles.cache.find(ro => ro.name == 'Muted');
if (!muteRole) {
    return message.channel.send("** انا لا أجد رتبة `Muted`**")
};
 
if(!mention) return message.channel.send(`**Ex : ${prefix}mute @user**`);
message.guild.channels.cache.forEach(c => {
c.updateOverwrite(role , {
SEND_MESSAGES: false, 
ADD_REACTIONS: false
});
});
mention.roles.add(role)
const embed = new Discord.MessageEmbed()
.setThumbnail(mention.user.avatarURL())
.setColor("GREEN")
.setTitle("Done ✅")
.setDescription(`**تــم أسكاته ${mention.user.username}**`)
.setFooter(`بــواسطة ${message.author.username}`)
message.channel.send(embed)
}
});

client.on('message', message => {
  if (!message.guild) return;
  if (message.content.startsWith( prefix + 'ban')) {
        if (!message.guild.member(message.author).hasPermission("KICK_MEMBERS"))
      return message.reply("**You Don't Have ` KICK_MEMBERS ` Permission**");
    if (!message.guild.member(client.user).hasPermission("KICK_MEMBERS"))
      return message.reply("**I Don't Have ` KICK_MEMBERS ` Permission**");      
 
    const user = message.mentions.users.first();
  
    if (user) {
      
      const member = message.guild.member(user);
      
      if (member) {
 
        member
          .ban({
            reason: 'They were bad!',
          })
          .then(() => {
            
                        const embed = new Discord.MessageEmbed()
           .setColor("0F750E")
               .setFooter(`Developer :  ⚜ 𝐂𝐀𝐙𝐀⚜ `)

          .setTitle(`Successfully banned ${user.tag}`)
          message.channel.send(embed);
          })
          .catch(err => {
 
            message.reply('I was unable to ban the member');
           
            console.error(err);
          });
      } else {
       
        message.reply("That user isn't in this guild!");
      }
    } else {
      
      const embed = new Discord.MessageEmbed()
.setColor("FF0000")
.setTitle("``You didn't mention the user to ban!`` ❌")
message.channel.send(embed);
    }
  }
});

client.on('message', message => {
  if (!message.guild) return;
  if (message.content.startsWith( prefix + 'kick')) {
    if (!message.guild.member(message.author).hasPermission("KICK_MEMBERS"))
      return message.reply("**You Don't Have ` KICK_MEMBERS ` Permission**");
    if (!message.guild.member(client.user).hasPermission("KICK_MEMBERS"))
      return message.reply("**I Don't Have ` KICK_MEMBERS ` Permission**");
    const user = message.mentions.users.first();
    if (user) {
      const member = message.guild.member(user);
      if (member) {
        member
          .kick('Optional reason that will display in the audit logs')
          .then(() => {
          
        
            const embed = new Discord.MessageEmbed()
           .setColor("0F750E")
               .setFooter(`Developer :  ⚜ 𝐂𝐀𝐙𝐀⚜ `)

          .setTitle(`Successfully kicked ${user.tag}`)
          message.channel.send(embed);
 
          })
          .catch(err => {
 
            message.reply('I was unable to kick the member');
            
            console.error(err);
          });
      } else {
       
        message.reply("That user isn't in this guild!");
      }
      
    } else {
 
const embed = new Discord.MessageEmbed()
.setColor("FF0000")
.setTitle("``You didn't mention the user to kick!`` ❌")
message.channel.send(embed);
    }
  }
});

client.on('message',async message =>{
let command = message.content.split(" ")[0]
command = command.slice(prefix.length)
if (message.content === prefix + "unlock") {
  if (!message.channel.guild)
    return message.reply("**this command is only for servers**");

  if (!message.member.hasPermission("MANAGE_GUILD"))
    return message.reply("**you don't have permissions **``MANAGE_MESSAGES``");
  message.channel.overwritePermissions([
{
 id: message.guild.id,
 allow: ['SEND_MESSAGES'],
},
], 'Needed to change permissions')
   message.channel.send(`**:unlock:| ${message.channel} Has Been Unlocked. **`)

}

if (message.content === prefix + "lock") {
  if (!message.channel.guild)
    return message.reply("**this command is only for servers**");

  if (!message.member.hasPermission("MANAGE_GUILD"))
    return message.reply("**you don't have permissions** ``MANAGE_MESSAGES``**");
  message.channel.overwritePermissions([
{
 id: message.guild.id,
 deny: ['SEND_MESSAGES'],
},
], 'Needed to change permissions')
      message.channel.send(`**:lock:| ${message.channel} Has Been Locked.**`)


}
});
client.on('message', message =>{
if(message.content === prefix +"hide"){
if(!message.member.hasPermission('MANAGE_CHANNELS')) return message.reply(' ** You dont have `MANAGE_CHANNELS` permission **');
let everyone = message.guild.roles.cache.find(hyper => hyper.name === '@everyone');
        message.channel.createOverwrite(everyone, {
              VIEW_CHANNEL : false
            }).then(() => {
                                const embed = new Discord.MessageEmbed()
                .setColor("RANDOM")
               .setThumbnail(message.guild.iconURL())
                .setDescription(`> **Done Hide This Room ${message.channel}**`)
                .setFooter(`By ${message.author.username}`)
                message.channel.send(embed)
                })
}
});

client.on('message', message =>{
if(message.content === prefix +"show"){
if(!message.member.hasPermission('MANAGE_CHANNELS')) return message.reply(' ** You dont have `MANAGE_CHANNELS` permission **');
let everyone = message.guild.roles.cache.find(hyper => hyper.name === '@everyone');
        message.channel.createOverwrite(everyone, {
              VIEW_CHANNEL : true
            }).then(() => {
                                const embed = new Discord.MessageEmbed()
                .setColor("RANDOM")
               .setThumbnail(message.guild.iconURL())
                .setDescription(`> **Done Show This Room ${message.channel}**`)
                    .setFooter(`Developer : ⚜ 𝐂𝐀𝐙𝐀⚜ `)

                })
}
});

client.on('message', function(message) {
    if(message.content.startsWith(prefix + "say")) {
      let say = message.content.split(" ").slice(1).join(" ");
      message.channel.send(`${say}`)
      message.delete()
 
}
});



client.on('message', badboy => {
  var args = badboy.content.split(' ').slice('1').join(" ")
  if(badboy.content.startsWith(prefix + "embed")){
    
 if(badboy.author.bot || !badboy.guild) return badboy.reply("this command for server only")
 if(!badboy.member.hasPermission("MANAGE_GUILD")) return badboy.channel.reply("you dont have a permission")
     var embed = new Discord.MessageEmbed()
    .setDescription(`${args}`)
    .setColor('RANDOM')
    badboy.channel.send(embed)
  }
})

const DIG = require("discord-image-generation");
client.on("message", async (message) => {
    if (message.content.startsWith(prefix + "spank")) {
              let user = message.mentions.users.first();
                            if(!user) return message.reply("need mention user")

        let avatar = message.author.displayAvatarURL({ dynamic: false, format: 'png' });
        const avatar2 = user.displayAvatarURL({ dynamic: false, format: 'png' });
        let img = await new DIG.Spank().getImage(`${avatar}`, `${avatar2}`);
        let attach = new Discord.MessageAttachment(img, "Spank.png");;
        message.channel.send(attach)
    }
});

client.on("message", async (message) => {
    if (message.content.startsWith(prefix + "rip")) {
              let user = message.mentions.users.first();
                            if(!user) return message.reply("need mention user")

        const avatar2 = user.displayAvatarURL({ dynamic: false, format: 'png' });
        let img = await new DIG.Rip().getImage(`${avatar2}`);
        let attach = new Discord.MessageAttachment(img, "Ri.png");;
    }
});

     
client.on('message', function(message) {
    if(message.content.startsWith(prefix + "vote")) {
      let arg = message.content.split(" ").slice(1).join(" ");
      if (!arg) return message.channel.send(`**Ex : ${prefix}vote Make Video ? **`);
const embed = new Discord.MessageEmbed()
.setColor("#f6ff00") 
.setAuthor(client.user.username,client.user.avatarURL())
.setThumbnail(message.author.avatarURL())
.setDescription(`${arg}`)
.setFooter(`React 👍 or 👎 | By ${message.author.username}`)
message.channel.send({embed}).then(msg => {
  msg.react('👍').then( r => {
    msg.react('👎')
  })
})
    }
});



client.on('message', message => {
    if (message.content.startsWith(prefix + 'kill')) {
        let user = message.mentions.users.first();
        if (!user) {
        }
        let kill = [
            'https://media.giphy.com/media/9tXn7DEOsjifNDEenF/giphy.gif',
            ``
        ];
        message.channel.send({
            embed: new Discord.MessageEmbed().setImage(
                kill[Math.floor(Math.random() * kill.length)]
            )
        });
    }
});

client.on("message", async (message) => {
let DIG = require("discord-image-generation");
    if (message.content.startsWith(prefix + "trash")) {
              let user = message.mentions.users.first();
                            if(!user) return message.reply("need mention user")
 
        const avatar2 = user.displayAvatarURL({ dynamic: false, format: 'png' });
        let img = await new DIG.Trash().getImage(`${avatar2}`);
        let attach = new Discord.MessageAttachment(img, "Trash.png");;
        message.channel.send(attach)
    }
});
     
client.on("message", async (message) => {
let DIG = require("discord-image-generation");
    if (message.content.startsWith(prefix + "delete")) {
              let user = message.mentions.users.first();
              if(!user) return message.reply("need mention user")
        let avatar = message.author.displayAvatarURL({ dynamic: false, format: 'png' });
        const avatar2 = user.displayAvatarURL({ dynamic: false, format: 'png' });
        let img = await new DIG.Delete().getImage(`${avatar2}`);
        let attach = new Discord.MessageAttachment(img, "Delete.png");;
        message.channel.send(attach)
    }
});
//-----------------------------------------------\\

client.on('ready', () => {
  console.log('-----------------------------------')
  console.log(`${client.user.username}: Im ready, my prefix is [ ${client.prefix} ] s! `)
  console.log('-----------------------------------')
  client.user.setActivity(' ⚜ 𝐂𝐀𝐙𝐀⚜ s!')
})
