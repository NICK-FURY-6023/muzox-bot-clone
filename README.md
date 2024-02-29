# muzox-bot-clone



A Discord Music bot project broughtto  

## Tech Stacks Information 

**Client:** Discord.js as Client library , Soukaku as Player library, Lavalink as Node server as player component 

**Language:** Typescript 


## Quick View Table

```http
  Quick View table 
```

| Version | implementation     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `V3`      | `Typescript Migration` | This version is a major change due to integration and migration to Typescript from javascript |

## 🔧 Requirements

Before starting , you would require some of the following stuff 

- ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white) [Install from here!](https://nodejs.org/en/download/)
- ![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white) [Download Here](https://www.mongodb.com/try/download/community)
- ![Lavalink](https://img.shields.io/badge/Lavalink-7289DA?style=for-the-badge&logo=fire&logoColor=white) [install from here](https://github.com/freyacodes/Lavalink)

## 📚 Steps 
1. Clone the repo
```bash 
git clone <repo url>
```
3. Navigate to the folder 
2. Open cmd in the following folder created & run
```bash 
npm install
```
3. After the complete installation open the folder containing the repo in your code editor 
4. Edit the file ```.env.example``` to ```.env```
5. Fill in the details required 
```js


Token="xxxxxxxxxx" # paste your Discord bot token
PostgresqlDb="" # Postgresql database url
TopGGApiKey="" # Top.gg api key
status="online" # online,dnd,idle,offline
Dprefix=" " # Prefix for your discord bot
SearchEngine="ytsearch" # soundcloud : scsearch , ytMusic : ytmsearch , yt : ytsearch
BotUsername=" " # Discord bot username
BotIcon="null" # Do not replace [future use]
BotUserId=" " # Your Discord bot user id
GuildLogs=" " # Your Discord channel id where guild Joined / Left events would trigger
ShardLogs=" " # Paste your ChannelId where to send the Shard realted events
ShardAlerts=" " # Paste your ChannelId where to send Shard alert events
ReadyLogs=" " # Paste Your ChannelId where to send Bot Ready Events
OwnerIds="943530917748691005, 1014198346656792667" # Developers Ids for dev acess commands 
MaintenanceReason="Currently the bot seems to be facing the maintenance mode" # Maintenance mode reason [to notify users when cmd is triggered & maintenace : True]
Estimation="Estimated : 12.00 am" # Maintenance mode time / string estimations

LavalinkUrl="xxx:5432" # Lavalink url format : [host:port] : [xxxx:1234]
LavalinkAuth="youshallnotpass" # Lavalink password
LavalinkName="Main" # Lavalink name [any]
```
you can delete the lines containing `not required`
You can disable the logging system for channels from the file `Src/config.ts [Line: 42]`
you can activate or deactivate maintenace from the file `Src/config.ts [Line: 48]`


6. generate the prisma Client 
```bash 
npx prisma generate
```
7. Lastly you can run the bot from the following cmd line
```bash
npm run dev
```
## useful files
1. you can update the txt of every message from the file
```Src/Display/Messages/Messages.ts```

2. you can update few embeds from the files in the folder 📂 
```Src/Display/GlobalEmbeds ```
