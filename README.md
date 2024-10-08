<h1>Silence of the Siren - Quick Translator's Guide</h1>

Thanks for visiting the translation project of Silence of the Siren! If you'd like to participate, here's a short guide to get you started.

<h2>Editing</h2>

Feel free to edit the files directly here on Github (browse to a file, 'pencil' icon top right).
When you're done, commit your changes and in the next step click on Propose changes to create a branch and a "pull request" which we'll then accept. Feel free to edit only a part of a file, some of them are pretty big.

If you'd like to edit the files on your desktop, make sure you use an editor that understands XML, something like the (free) Notepad++. There are two ways how to access the files on your desktop, you can either use a git client or just download the whole repository as a zip file, edit your files and then copy their contents to the online editor on github.

<h2>Best practices for the actual translations</h2>

- For commonly used terms please check how these got translated in other files, it might make sense to make a little glossary file if you're the first one starting the translation.

- Try to keep similar length as the English original. A lot of text boxes get resized to fit the texts, but it's always safer not to make the translated versions much different in length (yes, this can sometimes be a challenge).

<h2>Formatting</h2>
We use quite a few different tags, like \n for new line and the following tags for bold/italics and some color codes. These should be pretty straightforward, try to preserve them in the translation.

Lines with more complex formatting use the following tags at the beginning and at the end, please make sure you don't break them. This is actually the most common error that gets made. :)

    <![CDATA[   and    ]]>

Examples of some formatting tags and of a colored text:

    <![CDATA[Now <b><i>do something</i></b>.\nThis is on the next line.]]>
    <![CDATA[<color=SOTS_COLOR_GOLD>Aura Coins</color> generated per phase at this base.]]>

Some texts have parameters like {1} and {2}, which means names or bits of other texts get inserted into them - make sure these stay there! It often makes sense to change the word order here though so the sentences sound natural.

<h2>Steam keys</h2>

As a small reward and to help the actual process we're offering up to 5 Steam keys for each language. This will also make sure that new translators will be able to test the translations directly in the game.
The rule is: everybody who submits a translated file (with at least 20 lines) will be eligible to get a key as long as there are any left for the language (from previous experience, less than 5 volunteers for a language is to be expected. 

We recommend to let others know you're working on the translation. We'll try to organize everything on the game's discord server:
https://discord.gg/DAeGEtqHNS

<h2>Testing in game</h2>

Find the Streaming Assets folder in your game install folder and copy all the files to a separate folder under Modules. The xmls themselvese need to sit in a Database subfolder, please have a look at for example LanguagePackCZ.

If the game fails to load or if some of the translated texts don't show up, it's quite likely there's an issue with the xml/formatting tags. Checking the log file from the game can help.

Please check if all texts fit, if not, the issue might be on the side of the game, so please let us know!


