#**How to make your own custom app launcher with html**\
**WARNING**\
ANYTHING DONE WRONG CAN RESULT IN DAMAGE TO YOUR OPERATING SYSTEM. THIS ONLY WORKS ON WINDOWS

Open Registry editor with Windows + R or by searching in search
\
![Select HKEY_CLASSES_ROOT](https://raw.githubusercontent.com/BoxyPlayz/URLauncher/main/reg.png)\
Then select HKEY_CLASSES_ROOT and right click on itIn the menu,  select New  -> Key. Name it what you want the protocol to be (e.g. roblox, fortnite, etc) On the right side, right click and go to New -> String Value.
Rename it to  `URL Protocol`. While you have the first key selected, create another key called `shell`, and a third inside of the second called `open`.  Finally, create the final key inside of `open` called `command`.
You should have a tree that looks like this
\
![mine>shell>open>command](https://raw.githubusercontent.com/BoxyPlayz/URLauncher/main/tree.png)\
Finally, in command set thedefault value to ``"YOUR EXE FILEPATH HERE" "%1"``
Yes, you need the "%1" too. Now press ctrl + s to save and go to the protocol's name plus `://` for example, `roblox://` in your web browser.

