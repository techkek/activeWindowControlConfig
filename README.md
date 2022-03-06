# activeWindowControlConfig 
## English
This is my custom configuration for [Active Window Control](https://github.com/KDE/plasma-active-window-control), a very useful [KDE](https://kde.org) plugin for optimizing screen space, removing the minimize, maximize or close buttons, and placing them in the KDE panel.
### Installation
[Active Window Control](https://store.kde.org/p/998910) must first be installed. [AUR](https://aur.archlinux.org/packages/plasma5-applets-active-window-control-git)
```
cd /.local/share/plasma/plasmoids/org.kde.activeWindowControl
sudo rm -rf *
git clone https://github.com/techkek/activeWindowControlConfig.git
sudo mv activeWindowControlConfig/* . && sudo rm -rf activeWindowControlConfig
```
### Panel
This configuration is part of my [KDE panel](https://github.com/techkek/kekPanel).
### Small screens
:warning: If you have a small monitor, change the value
```
 <entry name="horizontalScreenWidthPercent" type="Double">
  <default>0.1</default>
</entry>
```
in ```contents/config/main.xml``` with a value greater than 0.1, otherwise you will not be able to select the applet.
### How does it work?
The applet only works when a window is full screen on a screen. In this way, the buttons to minimize, maximize or close the window will automatically disappear; if you move the cursor to the right of the clock, the three cursors will appear.
## Italiano
Questa è la mia configurazione personalizzata per [Active Window Control](https://github.com/KDE/plasma-active-window-control), un plugin di [KDE](https://kde.org) molto utile per ottimizzare lo spazio nello schermo, rimuovendo i tasti per ridurre a icona, massimizzare o chiudere a icona, e posizionandoli nel pannello di KDE.
<br>
### Installazione
Bisogna prima aver installato [Active Window Control](https://store.kde.org/p/998910) [AUR](https://aur.archlinux.org/packages/plasma5-applets-active-window-control-git)
```
cd /.local/share/plasma/plasmoids/org.kde.activeWindowControl
sudo rm -rf *
git clone https://github.com/techkek/activeWindowControlConfig.git
sudo mv activeWindowControlConfig/* . && sudo rm -rf activeWindowControlConfig
```
### Pannello
Questa configurazione fa parte del mio [pannello di KDE](https://github.com/techkek/kekPanel).
### Schermi piccoli
:warning: Se hai un monitor di dimensioni ridotte, modifica il valore 
```
 <entry name="horizontalScreenWidthPercent" type="Double">
  <default>0.1</default>
</entry>
```
nel file ```contents/config/main.xml``` con un valore più grande di 0.1, altrimenti non riuscirai a selezionare l'applet.
### Come funziona?
L'applet funziona solo quando su uno schermo una finestra è a schermo intero. In questo modo, automaticamente scompariranno i pulsanti per minimizzare, massimizzare o chiudere la finestra; se si sposta il cursore a destra dell'orologio appariranno i tre cursori.

