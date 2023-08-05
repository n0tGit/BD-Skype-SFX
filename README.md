# BD-Skype-SFX
Skype-styled SFX for BetterDiscord's NotificationSounds plugin.
The following processes will assume you've downloaded all of the sounds.
To do so, you can simply click the green "Code" button and "Download ZIP"; un-zip anywhere you want, using 7-Zip or WinRAR.

## Setup NotificationSounds
1. Go to Settings.
2. Head to plugins and Search "NotificationSounds".
   - If you don't have it installed, download it [here](https://betterdiscord.app/plugin/NotificationSounds).
   - Check [BetterDiscord's Documentation](https://docs.betterdiscord.app/users/#plugins) to see how to install plugins.
3. Click the cog button. You should read "Settings" when hovering your cursor on it.
4. Open the "Add new sound" category.
5. In "CategoryName", either use this repo's name, or use another name of your choice.
   - It is recommended that every file you add from this repo should have the same category name; this way it'll be easier to find.
6. In "SoundName", use the file's name.
   - You can use other names, but I recommend you use the file's name in order for the plugin to auto-assign the sound to its configuration.
   - Example: For the "Message Mentioned (\@everyone)" notification, name it "Mention2".
7. In "Source", press the "Browse File" button, then go to where you downloaded your sounds, and select your file.
   - Example: For the "Message Mentioned (\@everyone)" notification, use the "MsgMention Everyone" file.
8. Once you're done with your sound category, close the "Add new sound" category and open the "Sound config." category.
9. Find the notification name and click the category Combo Box.
10. Select the category you created in step 5.
11. Select the sound you added in step 6.
    - As I mentioned before, the plugin should be able to auto-assign it when you select the category. Either the default sound name has changed, or your sound name was written incorrectly.
12. Once you're done, click the "Done" button.

## Setup FriendNotifications
For now, this repo contains two additional audio files for the FriendNotifications plugin. The process is (somehow) less difficult.

1. Go to Settings.
2. Head to plugins and Search "NotificationSounds".
   - If you don't have it installed, download it [here](https://betterdiscord.app/plugin/FriendNotifications).
   - Check [BetterDiscord's Documentation](https://docs.betterdiscord.app/users/#plugins) to see how to install plugins.
3. Click the cog button. You should read "Settings" when hovering your cursor on it.
4. Open the "Notification Sounds" category.
5. Find the "Toast-Online" section and press the "Browse file" button.
6. Go to where you downloaded your sounds, and select the "Contact Online" file.
   - Repeat Step 5 and 6 for "Desktop-Online".
7. Repeat Step 5 and 6 for "Toast-Offline" and "Desktop-Offline". Use the "Contact Offline" file.
8. Click the "Done" button.

### To-do:
- Rename files
- Make a script for NotificationSounds?
- Update this Readme
