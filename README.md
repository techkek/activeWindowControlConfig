# activeWindowControlConfig
## Italiano
Questa è la mia configurazione personalizzata per [Active Window Control](https://github.com/KDE/plasma-active-window-control), un plugin di [KDE](https://kde.org) molto utile per ottimizzare lo spazio nello schermo, rimuovendo i tasti per ridurre a icona, massimizzare o chiudere a icona, e posizionandoli nel pannello di KDE.
<br>
### Installazione
Bisogna prima aver installato [Active Window Control](https://store.kde.org/p/998910) [AUR](https://aur.archlinux.org/packages/plasma5-applets-active-window-control-git)
'''
cd /.local/share/plasma/plasmoids/org.kde.activeWindowControl
sudo rm -rf *
git clone https://github.com/techkek/activeWindowControlConfig.git
sudo mv activeWindowControlConfig/* . && sudo rm -rf activeWindowControlConfig
'''
### Pannello
Questa configurazione fa parte del mio [pannello di KDE](https://github.com/techkek/kekPanel).
### Schermi piccoli
:warning: Se hai un monitor di dimensioni ridotte, modifica il valore 
```
 <entry name="horizontalScreenWidthPercent" type="Double">
  <default>0.1</default>
</entry>
```
con un valore più grande di 0.1, altrimenti non riuscirai a selezionare l'applet.
###Come funziona?
L'applet funziona solo quando su uno schermo una finestra è a schermo intero. In questo modo, automaticamente scompariranno i pulsanti per minimizzare, massimizzare o chiudere la finestra; se si sposta il cursore a destra dell'orologio appariranno i tre cursori.

