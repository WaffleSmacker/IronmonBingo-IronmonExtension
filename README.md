# IronmonBingo-IronmonExtension
An Ironmon Tracker extension: Enables Bingo events to be automatically triggered when playing IronMon (FireRed only)
Created by [WaffleSmacker](https://www.twitch.tv/wafflesmacker)

## Shoutouts
- [SteVanLe](https://www.twitch.tv/stevanle) - For the inspiration to make this extension
- [utdzac](https://www.twitch.tv/utdzac) - For continuing to update the tracker and make all this possible

## Important Notes
This requires a bit of setup and is not as easily implemented as other IronMon Extensions.

## Requirements
- [Ironmon-Tracker v8.4.1](https://github.com/besteon/Ironmon-Tracker) or higher
- [StreamerBot v.0.2.4](https://streamer.bot/api/releases/streamer.bot/latest/download) or higher

## Download & Install
1) Download the latest release of this extension from the GitHub's Releases page (coming soon)
2) If you downloaded a `.zip` file, first extract the contents of the `.zip` file into a new folder
3) Put the extension file(s) in the existing "**extensions**" folder found inside your Tracker folder
   - The file(s) should appear as: `[YOUR_TRACKER_FOLDER]/extensions/IronmonBingo.lua`
   - The folder should appear as: `[YOUR_TRACKER_FOLDER]/extensions/IronmonBingo`
4) On the Tracker settings menu (click the gear icon on the Tracker window), click the "**Extensions**" button
5) In the Extensions menu, enable "**Allow custom code to run**" (if it is currently disabled)
6) Click the "**Install New**" button at the bottom to check for newly installed extensions
   - If you don't see anything in the extensions list, double-check the extension files are installed in the right location. Refer to the [Tracker wiki documentation](https://github.com/besteon/Ironmon-Tracker/wiki/Tracker-Add-ons#install-and-setup-1) if you need additional help
7) Click on the "**IronMonBingo**" extension button to view the extension and turn it on

![image](https://github.com/user-attachments/assets/b51ae62b-04fb-4092-9b85-c3c314d7db6b)
![image](https://github.com/user-attachments/assets/42d4c31f-9af2-471e-9721-ce90878ecedc)

## Setup - Get the Stream Bingo Extension on Twitch:
[Stream Bingo](https://stream-bingo.com/)

1) Set up a new Bingo Card for Kaizo Ironmon
![image](https://github.com/user-attachments/assets/b9a3fab1-29da-4a0d-adce-9adb6ae2207d)

2) Get the values from the BingoEvents.txt file and create all of the events. (current count: 48)
![image](https://github.com/user-attachments/assets/5692d58e-40dc-424a-9323-59a0ad36a04a)
3) Get the webhook link from the Extension and add the link next to the coresponding event in the bingoLinks.json
![image](https://github.com/user-attachments/assets/9cf6d898-3e4b-40b6-a238-50b2d397010c)
4) Put the links here:
![image](https://github.com/user-attachments/assets/e3bf6a99-000d-47ad-8e77-4495c21ef5f7)

## StreamerBot Setup:
1) Open streamerbot
2) Click "Import"
![image](https://github.com/user-attachments/assets/d7661cf2-b8f2-4299-acb6-d981f091e22f)
3) Drag and Drop the "StreamerBot Settings" file into the import section.
![image](https://github.com/user-attachments/assets/349ae504-4692-4f37-88a1-4cafb2a14fa7)
![image](https://github.com/user-attachments/assets/a7357ac7-6a7a-4df7-a290-b26cd7861594)
4) Click "Import"
5) Go to "Trigger Bingo Event" Double click on "Execute Code"
![image](https://github.com/user-attachments/assets/4bcd6f54-e6f7-41b0-b4dc-0d463ab67f79)
6) Update the paths here to link to where your IronMon Extension is saved (I left my path there as a reference)
![image](https://github.com/user-attachments/assets/05e5c15b-fac2-4605-b4de-4905fb188ec1)
7) Hit "Save and Compile" on the bottom right.
8) Do the same for "Reset All Bingo Data"
![image](https://github.com/user-attachments/assets/6f9290d6-7e7c-4e5e-8edd-3eac8039c024)
![image](https://github.com/user-attachments/assets/8f592474-b2a7-41ad-bc2c-21ef52d8ebba)
9) Make sure the "!newbingo" command is enabled:
![image](https://github.com/user-attachments/assets/d1705860-4f9d-41ee-ae64-9c18d46d2bad)
10) Test the command in your chat:  !newbingo
11) If you get something like the following you are good to go:
![image](https://github.com/user-attachments/assets/0f25287c-ae6e-44a8-a759-d4fd1da30455)


## How to use
On your first use you will not need to do !newbingo.
The code will only trigger each even one time per bingo game.  It will automatically reset item counts when you start a new seed.
If you want to play a new game, make sure to do !newbingo to reset all of the existing data.
Simply turn off the extension if you don't want to use it anymore.
