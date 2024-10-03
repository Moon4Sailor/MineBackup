# MineBackup: Minecraft Worlds Backup Utility
**MineBackup** is a Windows Forms application designed to manage and back up Minecraft worlds from both Java and Bedrock editions. The app enables users to select and back up worlds to a designated folder while providing features like overwriting existing backups, viewing backup details, and deleting backups.

<div align="center">
    <img src="https://github.com/user-attachments/assets/3321e000-ae0d-4403-bb75-ff60a7d6e754" alt="Image description" width="400"/>
</div>


***
**Features**
**Supports Both Java and Bedrock Editions:** Users can choose between Minecraft Java or Bedrock edition to view and back up worlds.
**Backup Management:**
* List all Minecraft worlds, showing details like world name, size, seed, and creation date.
* Back up selected worlds with a click, avoiding duplication by replacing existing backups.
* **Backup List View:** View backed-up worlds and their details, such as backup date.
* **Delete Backups:** Remove selected backups from the backup folder.
* **Status Messages:** Display status updates, like backup progress or deletion confirmation.

**Prerequisites**
* Windows OS
* .NET Framework
* Minecraft installed (Java or Bedrock Edition)

***
## **Usage**
**Select the Platform:** Choose either Java or Bedrock from the dropdown.
* For Java, the app will look for worlds in the default _`.minecraft/saves`_ directory.
* For Bedrock, it will look for worlds in the default _`LocalState/games/com.mojang/minecraftWorlds`_ directory.

**View Worlds:** The application will display a list of worlds in the `ListView` with the following details
* Name
* Size
* Seed
* Creation Date

**Back Up Worlds:**
* Select worlds by checking the boxes.
* Click **Backup** to save them to the designated backup folder located in your Documents folder `(Documents/MinecraftBackups)`.
* If a world with the same name exists in the backup, it will be replaced.

View Backups: The second ListView will show all backed-up worlds with:
* Name
* Size
* Seed
* Backup Date

**Delete Backups:**
* Select the backups you wish to remove using the checkboxes.
* Click Delete to remove them from the backup folder and the list.

**Folder Structure**
* **Backup Folder:** All backups are saved in a folder called `MinecraftBackups` within the current user's Documents directory.

* **Backup Info File:** Backup metadata (world name, size, seed, and backup date) is saved in a `backups.txt` file within the backup folder for persistence across application runs.

**Error Handling**
* If the worlds directory is not found for the selected platform, an error message will be displayed.
* When backing up or deleting backups, appropriate error messages will be shown in case of issues.
***
Enjoy backing up your Minecraft worlds with MineBackup!



