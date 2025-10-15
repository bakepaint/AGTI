# How test ARMGDDN games

## Step 0 - Pre-requisites
We do test the games not as "ourselves", but as if we were a normal user. So we need to follow the tutorial. For testing we will always use:
- 7 ZIP
- The default folders (C:/Downloads and C:/Games)
- The AV exclusions as tutorial demands

We will not use anything besides that, like Open Composite, for example. Nor any other tool that can "mod" the way we play the games.

I will not teach how to install or setup nothing here, as you should have watched the tutorial already.

## Step 1 - Downloading the browser
I believe you alredy have it, right? RIGHT???

## Step 2 - Downloading the games
Now that you have the browser installed, let's download a game.

- First, you should check the `AG Testing` channel to see which games need testing
- Select a game from there. It's a good practice to send a message, saying that you took that game to test
  - There is no problem on testing a game already tested, but you usually wants to test a non-tested game
  - **NEVER CLAIM A GAME UNTIL YOU HAVE STARTED TO DONWLOAD IT**. I know that sometimes life calls and you end up not testing what you claimed to, but this can make other people skip this game and it ends up never being tested. Do not claim the game until you are 100% sure you WILL test in the same day (Even better if you claim and test it at the same time)
 
Now that you now the game you want to test, you can open the Staff browser. </br>
You should look for the "Untested - Coming Attractions" mirror, there you will find all games that need testing.
</br>
<img width="698" height="1027" alt="image" src="https://github.com/user-attachments/assets/4fe9db8b-9283-4ea7-a224-51c92c9a08c6" />
</br>
Open it, find the game you will test and simply right-click on it and download it, as you would normally do.

## Step 3 - First checks while the game download
To save some time, we can already test some stuff. So open the folder where the game is being downloaded and you will see the game id, for example `2314160` for Tactical Assault VR.
So, what you need to do is:
- Open https://steamdb.info/app/2314160/patchnotes (Remember to change the id for the real one you are testing)
- Check if the game it opened is really the one you are testing
- Check if the patch really exists and it's the last one
 - If it's not the last one, you can still test, but send a message on Telegram stating that's not the most recent version
</br>
<img width="1861" height="1033" alt="image" src="https://github.com/user-attachments/assets/bc7c6460-c4c1-4781-ad0c-5020f77404e8" />
</br>
If any of these info doesn't match, your test can end here. The repacker must fix the mismatched appids, version or wathever.

## Step 4 - Installing the game
- With the game downloaded, extract it using 7zip. You should already know how to do that...
- Open the installer, select language and let's go

Now, there are some oubvious to take note to see if it's correct:
- The splash when opening the installer should match the game
- The background of the installer should match the game
- Names, everything should match the game

Not-so-obvious things:
- Make sure AG Telegram button works and is redirecting to the correct place
- Make sure the Music button works
- Click on "?" on top right corner
  - Make sure game name and build id matches 
  - <img width="615" height="592" alt="image" src="https://github.com/user-attachments/assets/520613da-d57f-4577-a4e1-257ebb42b4db" />
  - Make sure AG Telegram button works and is redirecting to the correct place

If there is a missmatch, post it on the replies on Telegram and you can finish your test here.

You can now click on "Next" </br>
Here, write down the required disk space, in my case "12.20 GB"
</br>
<img width="610" height="463" alt="image" src="https://github.com/user-attachments/assets/84d46daa-9435-4c37-9eae-ce3bda84a406" />
</br>

- Click on "Install"
- Make sure all the images on background have good quality
- Make sure the Background button enable/disable the images

And it's this for now.

## Step 5 - Before starting the game
Remember the size you noted down? Let's check if it matches.
- Open the game install folder
- Right click on it --> Properties
- <img width="460" height="509" alt="image" src="https://github.com/user-attachments/assets/c3822d9d-5ef3-46a9-a0a1-335d03ac9d39" />
- Make sure the size matches
- While at it, check if the icons are present and in good quality
- Check ALL shortcuts, desktop and initial menu ones

Nice, now you can open the game folder and have a look, some important stuff you need to check
- You need to find a steam_appid.txt SOMEWHERE, sometimes are in the root and sometimes you will need to dig, but the file MUST be present (exceptions exists)
- Once you found it, make sure the appid is correct.
- <img width="1308" height="555" alt="image" src="https://github.com/user-attachments/assets/005a6e8c-8d86-4531-858e-653ba5e77429" />
- If you find anything strange or unusuall, post on Telegram.

## Step 6 - Testing the game itself
- Nice, now you can finally open the game. You should NOT use Open Composite or any other stuff on the games. Just test it as it's installed, raw. </br>
- For that, just open the shortcut that best matches your setup, in my case is VD (If the game is VR)</br> 
- Now, you need just to play a little to see if there are any problem. </br>
- Make sure to test all controls (Keyboard + Mouse AND Controller, if possible) (Here the keymaps are also important to test) </br>
- Check if the settings can be changed and if they keep changed after a restart </br>
- You can also test if the overlay works (Alt + tab), some repackers ship with it, others don't. It's a good test anyway </br>
- After all that, open the game again, check if its saving the progress </br>
- If you find any problem, post on Telegram. Some problems are repack related, but some are game-related. Anyway we don't want to post a problematic game. </br>
- Ok, so now that you tested the game itself, do the same AGAIN with all shotcuts available that are possible for you to test. (Don't forget about the start menu ones too!)

## Step 7 - Filling the report
You think it ended? THIN AGAIN </br>
We have a report to fill now: 
```
Internal DLL - We saw that on step 5, if you found nothing strange and there is the appid, then OK
Images / Logos / Slideshow - We saw that on step 4 and 5. All images, logos, icons, everything is OK?
Info Button - We saw this one on step 4, remember the "?" button? Was it OK?
Installer Music / Buttons / Links - All other stuff from Step 4, related to installer itself.
Size / Name of folder / Build id - Remember the size you noted down? If the folder was created correctly? It all goes here
Shortcuts - This one seems to be auto explanatory
Gameplay VR - This one also is auto explanatory. Does it works?
Gameplay Flat - If there is a flat version of the game, includes this line too

Additional Info - Anything else note worthy, I usually put here what I used to test
```

So, examples:
```
Internal DLL - OK
Images / Logos / Slideshow - Low quality slideshow images
Info Button - OK
Installer Music / Buttons / Links - OK
Size / Name of folder / Build id - OK
Shortcuts - Missing icon on desktop
Gameplay VR - Not great. The UI is too far, so when I try to pickup the public phone, for example, I can't read anything. When trying to fill the watering can, I can't open the tap. Hard to read the missions too, but this one was expected.
```

Great. Now just post it on Telegram and go to the next game \o/
