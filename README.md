# BanksiaGUI-Translation

Translations for the freeware Graphical User Interface [BanksiaGUI](https://banksiagui.com) based on the open source tournament manager for chess engines [Banksia](https://github.com/nguyenpham/Banksia) (named after an Australian native wildflower).



## Steps:

- Fork the repositories or Download Zip file
- Translate and try
- Upload: push to repository or send directly to us

## External tools:

You may ignore those tools since BSG translation source files are just text files thus a simple text editor may work well with them. However, the below tools can help:

Qt Linguist: this tool comes with Qt Creator thus we can’t download and use it separately. If you can, download that software (Qt Creator, it is a freeware with community version, at https://www.qt.io/) to use Linguist. It can help to speed up the translation significantly. It can convert your text files (translate sources) into binary files (with extension .qm) to use directly with BSG thus you can use immediately and/or check the translation

## Translate
Change the file bsg_en.ts into your language form:

Change filename: change the suffix from en to your language code which is two characters long. For example, Germany has language code is de and the country code is de too. Thus the file name should be renamed into bsg_de.ts
Set language-country code: open the translation source (text file), set up the header into new language-country code, in the example is de_DE:

```
<TS version=”2.1″ langugage=”de_DE”>
```

### Translate:

All English sentences between tags <source></source> should be translated into new language and store in next tags <translation></translation>. The property type=”unfinished” should be removed. You may ignore to translate if the English sentence is accepted by your language.

```
<message>
<location filename=”../../ui/dlg/activegamewidget.ui” line=”68″/>
<source>All games</source>
<translation>Alle Spiele</translation>
</message>
```
If you are using Qt Linguist, you can convert the translation source into binary by release function (menu -> File -> release). The tool will create a new file with extension .qm (bsg_de.qm). Just copy that file into the folder languages of BSG runnable file (for macOS, that folder is inside the packet BanksiaGUI). Restart BanksiaGUI and you can select your language from the main menu. Check, re-translate and re-try until you satisfy.


### Notes:
The German language package is work in progress (2779/4310 words). Feel free to contribute.
