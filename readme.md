# How to Test ARMGDDN Games

## Step 0 - Pre-requisites
We don't test the games as "ourselves"; we test them as if we were normal users. Therefore, we need to follow the tutorial. For testing, we will always use:
- 7-Zip
- The default folders (C:/Downloads and C:/Games)
- The AV exclusions as the tutorial demands

We will not use anything besides that, such as Open Composite or any other tool that can "mod" the way we play the games.

I will not teach you how to install or set up anything here, as you should have already watched the tutorial.

## Step 1 - Downloading the browser
I believe you already have it, right? RIGHT???

## Step 2 - Downloading the games
Now that you have the browser installed, let's download a game.

- First, you should check the `AG Testing` channel to see which games need testing.
- Select a game from there. It's good practice to send a message saying that you have taken that game to test.
  - There is no problem with testing a game that has already been tested, but you will usually want to test a non-tested game.
  - **NEVER CLAIM A GAME UNTIL YOU HAVE STARTED TO DOWNLOAD IT**. I know that sometimes life calls and you end up not testing what you claimed, but this can cause other people to skip this game, and it ends up never being tested. Do not claim the game until you are 100% sure you WILL test it on the same day. (It's even better if you claim and test it at the same time).
 
Now that you know the game you want to test, you can open the Staff browser. </br>
You should look for the "Untested - Coming Attractions" mirror; there you will find all games that need testing.
</br>
<img width="698" height="1027" alt="image" src="https://github.com/user-attachments/assets/4fe9db8b-9283-4ea7-a224-51c92c9a08c6" />
</br>
Open it, find the game you will test, and simply right-click on it and download it, as you would normally do.

## Step 3 - First checks while the game downloads
To save some time, we can already test some things. Open the folder where the game is being downloaded and you will see the game ID, for example, `2314160` for Tactical Assault VR.
What you need to do is:
- Open https://steamdb.info/app/2314160/patchnotes (Remember to change the ID to the real one you are testing).
- Check if the game that opened is really the one you are testing.
- Check if the patch really exists and if it's the latest one.
 - If it's not the latest one, you can still test, but send a message on Telegram stating that it's not the most recent version.
</br>
<img width="1861" height="1033" alt="image" src="https://github.com/user-attachments/assets/bc7c6460-c4c1-4781-ad0c-5020f77404e8" />
</br>
If any of this info doesn't match, your test can end here. The repacker must fix the mismatched appids, version, or whatever.

## Step 4 - Installing the game
- Once the game is downloaded, extract it using 7-Zip. You should already know how to do that.
- Open the installer, select the language, and let's go.

Now, there are some obvious things to take note of to see if they are correct:
- The splash screen when opening the installer should match the game.
- The background of the installer should match the game.
- Names and everything else should match the game.

Not-so-obvious things:
- Make sure the AG Telegram button works and redirects to the correct place.
- Make sure the Music button works.
- Click on "?" in the top right corner.
  - Make sure the game name and build ID match.
  - <img width="615" height="592" alt="image" src="https://github.com/user-attachments/assets/520613da-d57f-4577-a4e1-257ebb42b4db" />
  - Make sure the AG Telegram button works and redirects to the correct place.

If there is a mismatch, post it in the replies on Telegram, and you can finish your test here.

You can now click "Next". </br>
Here, write down the required disk space; in my case, "12.20 GB".
</br>
<img width="610" height="463" alt="image" src="https://github.com/user-attachments/assets/84d46daa-9435-4c37-9eae-ce3bda84a406" />
</br>

- Click "Install".
- Make sure all the images in the background are of good quality.
- Make sure the Background button enables/disables the images.

And that's it for now.

## Step 5 - Before starting the game
Remember the size you noted down? Let's check if it matches.
- Open the game's installation folder.
- Right-click on it -> Properties.
- <img width="460" height="509" alt="image" src="https://github.com/user-attachments/assets/c3822d9d-5ef3-46a9-a0a1-335d03ac9d39" />
- Make sure the size matches.
- While you're at it, check if the icons are present and are of good quality.
- Check ALL shortcuts: desktop and start menu ones.

Nice. Now you can open the game folder and have a look. Here are some important things you need to check:
- You need to find a `steam_appid.txt` file SOMEWHERE. Sometimes it is in the root folder, and sometimes you will need to dig, but the file MUST be present (exceptions exist).
- Once you've found it, make sure the appid is correct.
- <img width="1308" height="555" alt="image" src="https://github.com/user-attachments/assets/005a6e8c-8d86-4531-858e-653ba5e77429" />
- If you find anything strange or unusual, post it on Telegram.

## Step 6 - Testing the game itself
- Nice, now you can finally open the game. You should NOT use Open Composite or any other tools on the games. Just test it as it is installed, raw.
- To do that, just open the shortcut that best matches your setup—in my case, it's VD (if the game is VR). 
- Now, you just need to play for a little while to see if there are any problems.
- Make sure to test all controls (keyboard + mouse AND controller, if possible). (It is also important to test the keymaps here).
- Check if the settings can be changed and if they remain changed after a restart.
- You can also test if the overlay works (Alt + Tab). Some repackers ship with it, while others don't. It's a good test anyway.
- After all that, open the game again and check if it's saving the progress.
- If you find any problems, post them on Telegram. Some problems are repack-related, but some are game-related. In any case, we don't want to release a problematic game.
- Okay, so now that you've tested the game itself, do the same thing AGAIN with all available shortcuts that are possible for you to test. (Don't forget about the start menu ones, too!)

## Step 7 - Filling out the report
You think it's over? THINK AGAIN.
We have a report to fill out now: 
```
Internal DLL - We saw this in step 5. If you found nothing strange and the appid is present, then OK.
Images / Logos / Slideshow - We saw this in steps 4 and 5. Are all images, logos, icons, and everything else OK?
Info Button - We saw this one in step 4. Remember the "?" button? Was it OK?
Installer Music / Buttons / Links - All other items from Step 4 related to the installer itself.
Size / Name of folder / Build id - Remember the size you noted down? Was the folder created correctly? It all goes here.
Shortcuts - This one seems self-explanatory.
Gameplay VR - This one is also self-explanatory. Does it work?
Gameplay Flat - If there is a flat version of the game, include this line too.

Additional Info - Anything else noteworthy. I usually put what I used to test here.
```

For example:
```
Internal DLL - OK
Images / Logos / Slideshow - Low-quality slideshow images
Info Button - OK
Installer Music / Buttons / Links - OK
Size / Name of folder / Build id - OK
Shortcuts - The icon is missing on the desktop.
Gameplay VR - Not great. The UI is too far away, so when I try to pick up the public phone, for example, I can't read anything. When trying to fill the watering can, I can't open the tap. It's also hard to read the missions, but that was expected.
```

Great. Now just post it on Telegram and move on to the next game. \o/
