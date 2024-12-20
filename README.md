# Portfolio  
A collection of some personal projects developed over the years.

## Table of Contents  
1. [Alvis Online - Action MMORPG Game](#alvis-online---action-mmorpg-game)  
   - A scalable multiplayer game server infrastructure with features like user authentication, real-time updates, and cross-server communication.  
2. [Action Combat MMORPG Project](#action-combat-mmorpg-project)  
   - A successor to Alvis Online with overhauled infrastructure and enhanced gameplay mechanics.  
3. [Website for Selling Music Packs](#website-for-selling-music-packs)  
   - A visually engaging website for selling music packs built with Next.js and TailwindCSS.  
4. [Service App](#service-app)  
   - A modern peer-to-peer (P2P) marketplace for service-based transactions like repair and maintenance.  
5. [Foxpaw - 2D Action Platformer](#foxpaw---2d-action-platformer)  
   - An early game featuring monster battles, loot collection, and ability unlocking.  
6. [Guess The Breed](#guess-the-breed)  
   - A fun dog breed quiz game with over 300 breeds to identify.  
7. [SpeedPro App](#speedpro-app)  
   - A BLE-enabled app to control electric scooters without user tracking.  
8. [NClicker](#nclicker)  
   - An auto-click tool for Windows with advanced interval and randomization settings.  
9. [IniSharp Lite](#inisharp-lite)  
   - A lightweight .NET library for handling INI configuration files.  

---

## Alvis Online - Action MMORPG Game  

This project includes:  
- Game server  
- Central Server  
- PostgreSQL Database  
- Redis Caching  
- RabbitMQ  
- Game Client w/ Unity-native tools to dump map data and other things
- ASP.NET Core Web API
- Website
- Launcher / Updater
- WPF Tools to edit various game data  

### Project Overview  

A scalable multiplayer game server infrastructure designed for seamless interactions across multiple game worlds. It leverages modern .NET technologies and a customized version of DotNetty for networking, with support for Docker. Networking is implemented via a raw TCP stack using a custom protocol and the ISAAC stream cipher.

### Game Server  

The core component, responsible for handling individual game worlds. Features include:  
- Packet handling for communication.  
- Chat systems and private messaging.  
- Handshake protocols for secure connections.  
- User authentication, with multiple characters under the user.  
- Real-time player appearance, movement updating.  
- Inventory management, item bonuses, and descriptions.  

### Central Server  

Acts as the hub for cross-world communication and coordination. Responsibilities include:  
- Routing private messages between servers.  
- Managing game server registrations.  
- Ensuring seamless player interactions across worlds.  

### Media  

#### Videos  
- [Server-based Inventory](https://www.youtube.com/watch?v=ChpTJr-ekGk)  
- [Shops](https://www.youtube.com/watch?v=x-LcYwBIIDY)  
- [Account & Character Creation](https://www.youtube.com/watch?v=RIPgdxY_E2A)  

![image](https://github.com/user-attachments/assets/6a82bac9-2d2e-4245-a914-1c0eca357178)  
![image](https://github.com/user-attachments/assets/6768dca7-2bef-4f57-8814-50c2184d625f)

---

## Action Combat MMORPG Project  

A successor to **Alvis Online**, featuring overhauled server infrastructure and improved gameplay mechanics. Focused on scalability and efficiency using REST APIs for login and session management.  
- [Combat Example](https://www.youtube.com/watch?v=dIfHHXJaoVQ)  

![image](https://github.com/user-attachments/assets/6f67431b-46c6-4833-b6ea-f8d16902717b)  
![image](https://github.com/user-attachments/assets/d38b71bb-fff8-4a91-aa19-9d9b56d2d364)

---

## Website for Selling Music Packs  

Built with **Next.js** and **TailwindCSS**, this website features:  
- Custom animations when scrolling.  
- A custom music player.  

![image](https://github.com/user-attachments/assets/fc0c1ad6-c3ae-4053-8ea8-4860dea2af11)  

---

## Service App  

A modern peer-to-peer (P2P) marketplace for service-based transactions like repair and maintenance.  
- **Technologies:** .NET MAUI, ASP.NET Core Web API, PostgreSQL.  

![image](https://github.com/user-attachments/assets/8e58453f-573e-4ff1-9b5b-fb3f8c48d49a)  

---

## Foxpaw - 2D Action Platformer  

An early game from 2011 where players battle monsters, collect loot, and unlock new abilities.  

![image](https://github.com/user-attachments/assets/16c52834-324f-4cc1-af9e-b8c9f8095205)  

---

## Guess The Breed  

A fun quiz game challenging users to identify over 300 dog breeds.  

![image](https://github.com/user-attachments/assets/50d64557-acb8-450d-856a-aaf67777c4d9)  

---

## SpeedPro App  

Control an electric scooter via BLE without tracking users.  
- [Repository](https://github.com/Buryyy/SpeedPro)  

![image](https://github.com/user-attachments/assets/bdb23a06-308d-4023-979c-1eaa39599a8c)  

---

## NClicker  

An auto-click tool for Windows, supporting intervals, randomization, and presets.  
- [Repository](https://github.com/Buryyy/NClicker?tab=readme-ov-file)  

![image](https://github.com/user-attachments/assets/4b0927e4-a6a0-4f37-bb9c-04d0dfc2d2fe)  

---

## IniSharp Lite  

A lightweight .NET library for reading and writing INI configuration files.  
- [Repository](https://github.com/Buryyy/IniSharpLite)  
