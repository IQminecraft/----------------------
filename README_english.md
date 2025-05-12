# How to Download a World from a Bedrock Edition Server

### ※ Use at your own risk. I am not responsible for any issues.
### Also, <u>all newly added blocks will be replaced with coarse dirt</u>.

## Platforms Introduced
- Windows
  ※ Probably possible on environments where both Java and Bedrock Edition Minecraft can run.

## Requirements
- Java Account
- Bedrock Edition Account

## Prerequisites
- Knowledge of installing mods (Fabric)
- Knowledge of importing worlds in Java and Bedrock Edition

## Steps

### 0. Install je2be from the Microsoft Store (or website)
- [je2be Download Link](https://apps.microsoft.com/detail/9PC9MFX9QCXS?hl=ja-jp&gl=JP&ocid=pdpshare)

### 1. ViaProxy Setup

1.  **Download ViaProxy**
    -   Download "viaProxy-3.x.x-SNAPSHOT.jar" from here: [ViaProxy Download Link](https://build.lenni0451.net/job/ViaProxy/)
    -   (It's recommended to create a new folder)
    -   ※ Install Java beforehand so you can open .jar files.
2.  **Open ViaProxy**
    -   If it doesn't open, try using a .bat file.
3.  **Add an Account**
    -   Click on "Bedrock Account" and log in via your browser.
        ![image1](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image1.png)
4.  **Detailed Settings**
    -   Check "Ignore packet conversion errors" and "Fake resource pack acceptance".

### 2. Starting ViaProxy

1.  **Enter the server address in the "Server Address" field.**
    -   Enter in the format "IPAddress:Port" (without the quotes).
2.  **Set the "Server Version" field.**
    -   Select "Bedrock 1.21.x" (or the latest Bedrock version).
3.  **Set the "Minecraft Account" field.**
    -   Set to "Use selected account".
4.  **Click "Start" at the bottom.**
5.  **Confirmation of Success**
    -   Success is indicated by the display shown in the image below.

### 3. Setting up Minecraft

1.  **Create a 1.21.4 Fabric instance (recommended).**
2.  **Install the following mods:**

#### Required Mods
-   [Cloth Config API](https://www.curseforge.com/minecraft/mc-mods/cloth-config/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [Fabric Language Kotlin](https://www.curseforge.com/minecraft/mc-mods/fabric-language-kotlin/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)
-   [WorldTools: World Downloader](https://www.curseforge.com/minecraft/mc-mods/worldtools/files/all?page=1&pageSize=20&version=1.21.4&gameVersionTypeId=4)

### 4. Downloading the Server World

1.  **Launch Minecraft and add a server.**
    -   IP: `127.0.0.1:25568`
    -   ※ This is what is displayed when you start ViaProxy.
2.  **Join the server and move to the desired map.**
3.  **Press ESC and select "WorldTools".**
    -   Enter a name in the top field and press "start download".
        ![image2](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image2.png)
4.  **Move around to load all the chunks you want to download.**
5.  **Once all chunks are loaded, press ESC and click "save capture of {name}".**
6.  **Load the downloaded world in single-player.**
    -   If there are naturally breakable blocks like leaves, immediately execute `/tick freeze` and `/gamerule randomTickSpeed 0`.
7.  **Save the world and exit.**

### 5. Converting the World for Bedrock Edition

1.  **Select "Java Edition to" and "Bedrock Edition" and click "Next".**
2.  **Select the downloaded world by clicking "Select Other Folder".**
3.  **Click "Start".**
4.  **Choose "Save as mcworld".**
    ![image3](https://github.com/IQminecraft/how_to_download_a_map_from_bedrock_servers/blob/main/images/image3.png)

### 6. Importing the World in Bedrock Edition

1.  **Open the .mcworld file to import the world (or extract and copy it to the world folder).**
2.  **Open the world and you're done!**

## Final Notes
### Using this method on servers where it's not permitted is your own responsibility.
#### My experiences:
-   Placing or breaking blocks might get you kicked (incompatible).
-   Right-click items might not react or turn into chests; you might need to enter the world using a different method in such cases.
-   If there are many newly added blocks, they will be unusable (all will become coarse dirt).
-   If there are proxy servers, it's easier to get the server IP and PORT using Horizon.
-   Hive requires the direct IP, so here it is -> `139.99.116.122:19132`
