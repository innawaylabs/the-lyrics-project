# the-lyrics-project
Crowdsourcing and collaborating on a single source of truth for Lyrics.

All lyrics files should go in the Archive directory/folder in the root of the repo. The name of the file should follow the below convention.
* [Language Name]\_[Year Number]\_[Movie Name]\_[Song Title].xml

The internal format of the lyrics file should look like below example, at a high level:
```
<meta>
<tags>
</tags>
</meta>

<lyrics>
<hinglish>
Bicchhoo mere naina badi zahreeli ankh maare
</hinglish>
<hindi>
बिच्छू मेरे नैना बड़ी ज़हरीली आंख मारे
</hindi>
<meaning>
My eyes are like a scorpion, they throw very venomous glances[*]
</meaning>
<notes>
* - This line metaphorically describes the person's eyes as being as dangerous or captivating as a scorpion, with the ability to enchant or harm others through their gaze alone. The overall context of the lyric suggests allure and danger, a common theme in many songs to describe the mesmerizing effect of someone's beauty or glance on others.
</notes>
</lyrics>
```

Also create shortcut or symbolic link (using relative path) to each file in different directory hierarchies as per the below guidelines.
* Language/[Language_Name]/[Movie Name]/Year/
* Language/Mixed/
* Artist/[Artist Name]/
* Year/[Year Number]/
* Year/Unknown_Year/
* To_Be_Classified/


# Handy commands

## Command to create a bunch of directories for a new language or category you are initiating:
```
for i in {1900..2019}; do mkdir "$i"; done
```
