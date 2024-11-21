# Portfolio - of some personal projects over the years. 

# Alvis Online - Action MMORPG Game

This project includes:
- Game server
- Central Server
- PostgreSQL Database
- Redis Caching
- RabbitMQ
- ASP.NET Core Web Api
- WPF Tools to edit various data that the game has

# Project Overview

This project is a scalable multiplayer game server infrastructure designed to support seamless interactions across multiple game worlds. The system is built with performance and efficiency in mind, leveraging modern .NET technologies and a customized version of DotNetty for networking. Docker is supported for every piece of tech this infrastructure uses. The networking is done via raw TCP stack with my own networking protocol utilizing the ISAAC stream cipher.

## Game Server

The game server is the core component, responsible for handling individual game worlds. It is optimized with modern .NET features like `Span<T>` and `Memory<T>` to achieve high performance and efficient memory management. Each server supports key gameplay functionalities, including:

- Packet handling for communication.
- Chat systems and private messaging.
- Handshake protocols for secure connections.
- User authentication (login and registration).
- Player movement and real-time updates.
- Inventory management, item bonuses, and detailed item descriptions.

The architecture supports multiple game servers, or "worlds," running concurrently, ensuring scalability for large player bases.

## Central Server

The central server acts as the hub for cross-world communication and coordination. It handles tasks such as:

- Routing private messages (e.g., whispers) between players across different game servers.
- Managing the registration of game servers at startup to maintain a comprehensive view of the active game worlds.
- Ensuring seamless player interactions across servers by locating target players and relaying messages or actions efficiently.

This infrastructure provides a robust foundation for creating immersive multiplayer experiences with scalability and flexibility to adapt to evolving requirements.

## Media

### Videos
- Server-based Inventory: https://www.youtube.com/watch?v=ChpTJr-ekGk
- Shops: https://www.youtube.com/watch?v=x-LcYwBIIDY
- Account & Character Creation: https://www.youtube.com/watch?v=RIPgdxY_E2A

### Images
![image](https://github.com/user-attachments/assets/6a82bac9-2d2e-4245-a914-1c0eca357178)
![image](https://github.com/user-attachments/assets/53cd0f79-03a2-4859-984b-e2fdc17f2471)
![image](https://github.com/user-attachments/assets/556dc823-47cc-46f8-9606-a5039cff4d3b)
![image](https://github.com/user-attachments/assets/93254088-3047-45e5-b863-52e3e90c4bf9)
![image](https://github.com/user-attachments/assets/a357f383-362a-4f0b-ad44-b2e28adcbf0a)
![image](https://github.com/user-attachments/assets/14959f05-8eb6-4f80-af97-7ef70f6009f3)
![image](https://github.com/user-attachments/assets/6b3d0598-eb98-4013-8a1b-4ea9ff1f1097)
![image](https://github.com/user-attachments/assets/248adc6d-0694-4ad8-b108-12b2cb69a83c)
![image](https://github.com/user-attachments/assets/7f8216ca-7a25-417c-859b-b0535abc1e95)
![image](https://github.com/user-attachments/assets/6c80ca4b-efd5-4d2d-884a-b4580289da07)
![image](https://github.com/user-attachments/assets/cebb1260-61f9-48ea-8b71-99af62b2e4d0)
![image](https://github.com/user-attachments/assets/a9e53b53-b0c4-4e51-97ab-c20d4f5c06aa)
![image](https://github.com/user-attachments/assets/7de07d0a-ff5c-4510-8248-2334d09001ae)

Cache distribution fully automated, the game would load new cache file upon next start.
 <video src='https://github.com/user-attachments/assets/fbc2db36-b3a5-4122-8cb3-5b9c1a991ddb' width=180/>

Launcher updating procedure
<video  src='https://github.com/user-attachments/assets/16179682-beb3-4a24-aa8e-6edacc17b093' width=180/>

Item Editor
<video  src='https://github.com/user-attachments/assets/e0154164-d7cb-4974-9253-b867342eb5a6' width=180/> 
![image](https://github.com/user-attachments/assets/7bdbd86b-a9c2-4010-844f-d8257c651fd4)


Player Updating Example
![image](https://github.com/user-attachments/assets/2489eca2-4bf6-4631-89ed-1ec72abfcccf)

Launcher
![image](https://github.com/user-attachments/assets/311262d9-5ff9-4f78-8ec1-06cedc2c0069)

Server Data Tool for editing items,npcs, and various data of the game. Includes cache updating mechanism that is basically a huge encrypted LiteDB file that the game client uses, that's where the datas are stored and deployed.
![image](https://github.com/user-attachments/assets/503e6d14-b798-4112-8ace-99f5dc2b1ec4)
![image](https://github.com/user-attachments/assets/9a35cd0c-af45-4adb-bbb4-db38721a1122)
![image](https://github.com/user-attachments/assets/f3305ede-56ba-4593-82d5-42eb294d6bf8)
![image](https://github.com/user-attachments/assets/d7b089ca-0c89-4f63-b30c-5aca673adf6a)


# Unannounced Project - Currently working on this.

This project is in its early stages and serves as the successor to Alvis Online. I've opted for lower-poly graphics due to Unity Engine's limitations with high-fidelity rendering. The primary goal is to improve every aspect of the game, including a completely overhauled server infrastructure. Currently, I'm focusing on the login system, where all processes—login, character creation, and session management—are handled entirely through a REST API for efficiency and scalability.
- Combat example: https://www.youtube.com/watch?v=dIfHHXJaoVQ
  
![image](https://github.com/user-attachments/assets/6f67431b-46c6-4833-b6ea-f8d16902717b)
![image](https://github.com/user-attachments/assets/d843449c-9430-4a65-86ef-a211e9ed75be)

 # Website for selling music packs for game engine asset stores

I have used Next.js and tailwindcss for this website, it includes custom animations when scrolling, custom music player.
![image](https://github.com/user-attachments/assets/fc0c1ad6-c3ae-4053-8ea8-4860dea2af11)
![image](https://github.com/user-attachments/assets/073acd2e-3552-44e2-ae54-85d3581aff25)


# Service App
This project aimed to create a modernized peer-to-peer (P2P) marketplace platform, similar to Tori.fi. However, it focused on enabling individuals to offer services such as backyard maintenance, repair work, and more, allowing users to connect and transact directly for service-based needs. The application was made with .NET MAUI following modern .NET architecture. As for backend, this app was using Asp.Net Core Web Api w/ identity server and PostgreSQL for database.

![343438472_209936008480678_5893315607928065494_n](https://github.com/user-attachments/assets/8e58453f-573e-4ff1-9b5b-fb3f8c48d49a)
![344785348_781154036990992_6117082252079210398_n](https://github.com/user-attachments/assets/344fb3f2-b5eb-4ca7-b395-3a1d7570ee76)

# Foxpaw - 2D Action Platformer
This is one of my earlier games, created around 2011. Players embark on an adventure battling monsters, collecting loot, exploring diverse maps, and unlocking new abilities, providing an engaging progression experience.
![2f2e89f1a65409795dc66983910c9c21](https://github.com/user-attachments/assets/16c52834-324f-4cc1-af9e-b8c9f8095205)
![bbf2f09e5610b0bd7cc9b54d959e985d](https://github.com/user-attachments/assets/dfd2e672-7fa7-43af-9fbc-4b1ee09df6cb)
![ac49edecc03ee6966c9ddf5b32c5c5d1](https://github.com/user-attachments/assets/17785384-8064-4923-bddd-9c099f1b96b4)
![bc8862537582ef028f0f4643ba5e4181](https://github.com/user-attachments/assets/06f93116-678f-4400-8686-d6a968eb78e7)
<video  src='https://github.com/user-attachments/assets/489cdb19-8018-4023-9357-cd167daf2339' width=180/>  
<video  src='https://github.com/user-attachments/assets/88f1d769-08a3-46ad-b12f-e3241bc3203f' width=180/>  

# Guess The Breed
A simple and fun dog breed quiz game that challenges your ability to recognize over 300 different dog breeds.

![118110864_778558999584280_2704248700642941756_n](https://github.com/user-attachments/assets/50d64557-acb8-450d-856a-aaf67777c4d9)
![118374390_1699218326883434_864894154088761500_n](https://github.com/user-attachments/assets/e5ba5e93-1bce-48aa-9539-58383e1b4a94)
![unknown](https://github.com/user-attachments/assets/f025d052-f802-4dd7-9af1-245345bdcfef)




