# DarkSouls3SaveGameBackupTool

A program that creates backups of your Dark Souls 3 save every 15 minutes by default. Can customize the back up time interval to be between 1 to 59 minutes.

Back ups are created in the following format (hours in 24HR military time format):

`Month_Day_Year_Hour_Minute__DS30000.sl2.bak`

Like so: `5_2_2016_10_03__DS30000.sl2.bak`

To restore a backup, delete your `DS30000.sl2` file and rename the backup of your choice to `DS30000.sl2`.

Please note that you will start the backup process by pressing the "Start" button. Then start up Dark Souls 3 and play.

When you are done playing, press the "Stop" button.

### [Download Dark Souls 3 Save Game Backup Tool](http://www.nexusmods.com/darksouls3/mods/16?)

#### [Virus Total](https://www.virustotal.com/en/file/7cd31e90694bbe896272e5c81eca0762cb5f860ad926077c3673ba2e3a4a2253/analysis/1462494364/)

Important note: Do not delete or remove the `DarkSouls3SaveGameBackupTool.exe.config` file. This stores the time interval setting. It must be in the same folder as the `DarkSouls3SaveGameBackupTool.exe` file.

![DarkSouls3SaveGameBackupTool](https://github.com/insane0hflex/DarkSouls3SaveGameBackupTool/blob/master/Images/example.png)

### ToDos
- ~~Store TimeInterval setting for user~~
- ~~Make back up file name built with a human readable date rather than .ToFileTime()~~
- ~~Prettify the UI~~
- ~~Better code comments~~
- ~~Create a check for the `.exe.config` file and create it if it doesn't exist~~
- ~~Restore save from backup feature (instead of user manually deleting the old save and renaming a backup to `DS30000.sl2`~~
- Keep a "MaxBackup" amount - like 10 - where older backups above 10 are automatically deleted.


### Build Instructions

Want to build from source?

Download/fork this repo then open the solution file (you will need Visual Studio installed with at least .NET Framework 4.0 installed) and build. You can get [Visual Studio Community](https://www.visualstudio.com/en-us/visual-studio-homepage-vs.aspx) for free. Once you build, the binary (.exe file) is located in /bin/Debug/ folder.


