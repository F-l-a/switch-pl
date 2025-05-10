Read this page when Nintendo releases a new firmware update.
There's probably a better way to do this. Treat this as just a suggestion.

1. Update your firmware.
2. Follow [Dumping the system menu](https://github.com/bandithedoge/switch-pl/wiki/1.-Dumping-the-system-menu) and [Extracting the dumps](https://github.com/bandithedoge/switch-pl/wiki/2.-Extracting-the-dumps) again. Put the files in a different folder.
3. **Install [Meld](https://meldmerge.org/)**.
    * Most major Linux distros should have Meld in their official repositories. Try installing `meld` with your package manager.
4. Run Meld and click on *Directory comparison*. Select the folders where you have titles from the latest firmware version and the last translated one. Click *Compare* and wait until Meld finishes finding differences.
5. You'll see 2 panes with each folder and their differences.
    * Green text means the file is new. Blue text means the file is changed.
6. Write down a list of changed and new files.
7. Take the changed MSBT files from the old firmware and add `.bak` to the end of their names. Put them in the same folder as the new MSBT files.
8. Open 2 Kuriimu windows - one with the new file and the other with the old one.
9. In the window with the new file start looking for strings which are different or missing in the old one. If a string is missing in the old file, go to the other Kuriimu window and add a string with the same name.
    * You can use Ctrl+A to add a new entry.
    * You can press Ctrl+R to bring up the rename prompt and copy the name.
10. Save the old file with the added strings. Delete the new file and remove `.bak` from the old one.
11. Follow [Testing your translation](https://github.com/bandithedoge/switch-pl/wiki/4.-Testing-your-translation) again.