# BD-Skype-SFX
Skype-styled SFX for BetterDiscord's NotificationSounds plugin.
The following guides will assume you've downloaded all of the sounds.
To do so, you can simply click the green "Code" button and "Download ZIP"; un-zip anywhere you want, using 7-Zip or WinRAR.

## Setup NotificationSounds
### Method 1 (Recommended) - "Semi-automatic":
0. Install NotificationSounds if you haven't already. Make sure it's enabled.
   - Download it [here](https://betterdiscord.app/plugin/NotificationSounds).
   - Check [BetterDiscord's Documentation](https://docs.betterdiscord.app/users/#plugins) to see how to install plugins.
1. Download the JSON file [here](https://github.com/n0tGit/BD-Skype-SFX/raw/main/NotificationSounds.config.json). Alternatively, you can download it [here](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/n0tGit/BD-Skype-SFX/blob/main/NotificationSounds.config.json) - I created this link using [Minhas Kamal](https://github.com/MinhasKamal)'s [DownGit](https://github.com/MinhasKamal/DownGit) website.
2. (On Windows) Go to %appdata%.
   - Method 1: Press Win+R and type "%appdata%".
   - Method 2: In the Start menu, search "%appdata%". A folder will appear, it may be named "Roaming" or just "%appdata%". Open it.
3. Find your BetterDiscord installation folder (not discord/discordcanary/discordptb).
4. Go to the plugins folder.
5. Move or copy the JSON file you downloaded to that folder.
   - You may be asked if you want to replace a file. Do replace it.
6. If Discord is running, restart it.

### Method 2 - Manual (copy-and-paste):
1. (On Windows) Go to %appdata% (see Method 1).
2. Find your BetterDiscord installation folder (not discord/discordcanary/discordptb).
3. Go to the plugins folder.
4. Open the Notification Sounds config JSON file.
   - If you can't find it, make sure the plugin is installed. If you can't still find it, make sure it's enabled and check its settings through Discord.
5. You'll see the following contents in your JSON file:
```
{
	"all": {
		"choices": {
			"activities-rocket-time": {
				"category": "---",
				"focus": false,
				"invisibleMute": false,
				"mute": false,
				"sound": "---",
				"streamMute": false,
				"volume": 100
			}, // There are more elements here, I just removed them for demonstration. This is why you see a comma.
		}
	}
}
```
You'll need to copy the following text:
```
   "audios": {
			"Skype": {
				"Call Calling": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/calling.mp3",
				"Call Ringing": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/ring1.mp3",
				"Deafen": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/Deafen.mp3",
				"Disconnect": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/Disconnect.mp3",
				"HotKeys Left": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/hk_left.mp3",
				"HotKeys Right": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/hk_right.mp3",
				"Invited To Speak": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/ring2.mp3",
				"Message": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/msg.mp3",
				"Message (Direct Message)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/msg_dm.mp3",
				"Message (Group Message)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/msg_dm.mp3",
				"Message Mentioned": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/mention_user.mp3",
				"Message Mentioned (@everyone)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/mention_everyone.mp3",
				"Message Mentioned (@here)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/mention_here.mp3",
				"Message Mentioned (reply)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/msg_reply.mp3",
				"Message Mentioned (role)": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/mention_role.mp3",
				"Mute": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/Mute.mp3",
				"Push2Talk Start": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/ptt_start.mp3",
				"Push2Talk Stop": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/ptt_stop.mp3",
				"Stream Ended": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/stream_end.mp3",
				"Stream Started": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/stream_start.mp3",
				"Stream User Joined": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/stream_join.mp3",
				"Stream User Left": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/stream_left.mp3",
				"Undeafen": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/Undeafen.mp3",
				"Unmute": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/Unmute.mp3",
				"Voice Channel User Join": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/user_join.mp3",
				"Voice Channel User Leave": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/user_leave.mp3",
				"Voice Channel User Moved": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/user_moved.mp3"
			}
		},
```
So your JSON file looks like this:
```
{
	"all": {
		"audios": {
			"Skype": {
				"Call Calling": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/calling.mp3",
			} // There are more elements here, I just removed them for demonstration.
		},
		"choices": {
			"activities-rocket-time": {
				"category": "---",
				"focus": false,
				"invisibleMute": false,
				"mute": false,
				"sound": "---",
				"streamMute": false,
				"volume": 100
			},
		}
	}
}
```
Note that if you added sounds before, the JSON file will already have an "audios´ element, and therefore you'll only have to copy this:
```
			"Skype": {
				"Call Calling": "https://github.com/n0tGit/BD-Skype-SFX/raw/main/calling.mp3",
			} // Again, there are more elements here. I'm not putting them all.
```
6. Save your file and, if running, restart Discord.
   - If you open the JSON file again, you'll notice it no longer has the links I provided. This is because of how the plugin works, and in theory, the files should be stored locally.

### Method 3 - Manual (one-by-one):
0. Download the sounds by clicking the green "Code" button, and selecting "Download ZIP".
   - Un-zip the sounds using 7-Zip or WinRAR.
2. Go to Settings.
3. Head to plugins and Search "NotificationSounds".
   - If you don't have it installed, download it [here](https://betterdiscord.app/plugin/NotificationSounds).
   - Check [BetterDiscord's Documentation](https://docs.betterdiscord.app/users/#plugins) to see how to install plugins.
4. Click the cog button. You should read "Settings" when hovering your cursor on it.
5. Open the "Add new sound" category.
6. In "CategoryName", either use this repo's name, or use another name of your choice.
   - It is recommended that every file you add from this repo should have the same category name; this way it'll be easier to find.
7. In "SoundName", use the file's name.
   - You can use other names, but I recommend you use the file's name in order for the plugin to auto-assign the sound to its configuration.
   - Example: For the "Message Mentioned (\@everyone)" notification, use the same name.
8. In "Source", press the "Browse File" button, then go to where you downloaded your sounds, and select your file.
   - Example: For the "Message Mentioned (\@everyone)" notification, use the "mention_everyone.mp3" file.
9. Click "Save".
10. Once you're done with your sound category, close the "Add new sound" category and open the "Sound config." category.
11. Find the notification name and click the category Combo Box.
12. Select the category you created in step 5.
13. Select the sound you added in step 6.
    - As I mentioned before, the plugin should be able to auto-assign it when you select the category. Either the default sound name has changed, or your sound name was written incorrectly.
14. Once you're done, click the "Done" button.

## Setup FriendNotifications
For now, this repo contains two additional audio files for the FriendNotifications plugin. The process is (somehow) less difficult.

1. Go to Settings.
2. Head to plugins and Search "FriendNotifications".
   - If you don't have it installed, download it [here](https://betterdiscord.app/plugin/FriendNotifications).
   - Check [BetterDiscord's Documentation](https://docs.betterdiscord.app/users/#plugins) to see how to install plugins.
3. Click the cog button. You should read "Settings" when hovering your cursor on it.
4. Open the "Notification Sounds" category.
5. Select one of the methods below.

### Use files (you need to download "[contact_online.mp3](https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_online.mp3)" and "[contact_offline.mp3](https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_offline.mp3)" | Alt: [1](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_online.mp3) & [2](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_offline.mp3)):
6. Find the "Toast-Online" section and press the "Browse file" button.
7. Go to where you downloaded your sounds, and select the "contact_online" file.
   - Repeat Step 5 and 6 for "Desktop-Online".
8. Repeat Step 5 and 6 for "Toast-Offline" and "Desktop-Offline". Use the "contact_offline" file.
9. Click the "Done" button.

### Use URLs:
6. Right click [this link](https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_online.mp3) and select "Copy link" or "Copy URL address".
7. Paste the link in "Toast-Online".
   - Do this as well for "Desktop-Online".
8. Repeat step 6 using [this link](https://github.com/n0tGit/BD-Skype-SFX/raw/main/contact_offline.mp3).
9. Repeat step 7 for both "Toast-Offline" and "Desktop-Offline".
See the "Use files" method for alternative download links.

### To-do:
- ~~Rename files~~
- ~~Make a script for NotificationSounds?~~ Not a script per-se, just a JSON file that saves you from adding sounds one-by-one. I won't do this for FriendsNotifications as I consider two sounds to be enough.
- ~~Update this Readme~~ Might do again.
- Add more sounds
