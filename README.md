# Statistik und Statistische Grafik<br>mit Office- und Statistiksoftware

### LV Nr 405.365


### Vorbereitung zur LV

Bitte bringen sie in die LV ihren Laptop mit, wir werden vieles gemeinsam während der LV machen.

#### Software
Installieren sie folgende Software:

R (von https://cran.r-project.org)
RStudio (von https://www.rstudio.com/products/rstudio/download/preview/)
und für Windows auch Rtools (ebenfalls von https://cran.r-project.org)

Unter Windows tun sie dazu folgendes:

Laden sie folgende Dateien herunter:

  * https://cran.r-project.org/bin/windows/base/R-3.5.1-win.exe
  * https://s3.amazonaws.com/rstudio-ide-build/desktop/windows/RStudio-1.2.1070.exe
  * https://cran.r-project.org/bin/windows/Rtools/Rtools35.exe

Zur Installation gehen sie so vor

  * Führen sie das Installationsprogramm heruntergeladene `R-3.5.1-win.exe` aus   
  * Im Installationsdialog dieses Programm machen sie folgendes:   
    -  Customize Startup Options
		*  SDI (separate Windows)
		*  HTML Help
		*  Create a desktop shortcut
		*  Save version number in registry
		*  Associate R with .RData file 
	* Führen sie das Installationsprogramm `Rtools35.exe` aus und akzeptieren sie die Standard-Einstellungen
	* Führen sie das Installationsprogramm `RStudio-1.2.1070.exe` aus
	* Wenn die Installation fertig ist starten sie `RStudio` vom Start Menu.
	* Nachdem RStudio läuft erscheint ein Icon im Taskbar. Klicken sie auf das Icon und führen sie `Pin to Taskbar` aus.

Die Installation der Programme ist jetzt abgeschlossen, aber es müssen noch einige Zusatzpakete in R bzw. RStudio installiert werden.

Kopieren sie dazu folgenden Code in das `Console`-Window von RStudio:

```
pkgs_to_install <- c(
"tidyverse",
"magrittr",
"ggmosaic",
"ggforce",
"gganimate",
"ggtree",
"ggExtra",
"gridExtra",
"ggthemes",
"ggThemeAssist",
"ggplot2movies",
"ggmap",
"ggrepel",
"ggwordcloud",
"egg",
"scales",
"sf",
"maptools",
"rgeos",
"pracma",
"readxl",
"writexl",
"Dykstra",
"quadprog",
"devtools",
"cowplot", 
"googleway", 
"ggplot2", 
"ggrepel", 
"ggspatial", 
"libwgeom", 
"rworldmap", 
"rworldxtra",
"rayshader",
"shiny",
"reprex",
"datapasta",
"tidytext"
)

install.packages(pkgs_to_install)
```
Danach führen sie folgenden Befehl aus 

```
devtools::install_github("thomasp85/patchwork")
devtools::install_github("mkearney/rtweet")
```


und führen sie diesen Code aus (dazu einfach Return drücken)


Wenn sie auf ihrem Rechner `TeX` noch nicht installiert haben, dann
führen sie auch folgenden Code aus:

```
install.packages("tinytex")
library(tinytex)
install_tinytex()
```




#### Github


Das Herunterladen der Materialien geht einfacher, wenn sie auch noch einen Github-Account (auf https://github.com) anlegen.

Das geht  auf dieser Seite: https://github.com/join?source=header-home

Wählen sie bei der Registrierung den `Free Plan` aus.

*Achtung: Free Plan heißt, dass ihre Dateien frei zugänglich sind.
Wenn sie das nicht wollen, dann dürfen sie keinen solchen Account anlegen.
Sie haben dann immer noch Zugang zu meinen LV-Dateien, können Github aber nicht selbst zum Speichern verwenden.*

Außerdem müssen sie `git` von hier       https://github.com/git-for-windows/git/releases/download/v2.19.1.windows.1/Git-2.19.1-64-bit.exe    
installieren.

Führen sie dann noch (in einem Command-Fenster) folgenden Befehl aus:   
`git config --global credential.helper wincred`

Wir benötigen auch Daten. Dazu laden sie bitte folgende Zip-Dateien auf ihren Rechner (wir werden die Daten in der LV benötigen).
*Achtung*: Die erste Datei ist relativ groß, ca 200 MB

  * https://myfiles.sbg.ac.at/index.php/s/8A4ShFkQ1E0liPq
  * https://myfiles.sbg.ac.at/index.php/s/7AtXdO0hqKziOaD

### Twitter

Wenn sie noch keinen Twitter-Account haben legen sie bitte einen an.     
Schicken sie mir bitte in beiden Fällen ihren Twitter-handle. Und folgen sie mir auf Twitter, mein Twitter-Handle ist `neuwirthe`




#### Andere Betriebssysteme

Wenn sie Linux oder MacOS verwenden Installieren sie bitte R und RStudio
von den genannten Websites (es gibt dort auch Versionen für diese Betriebssysteme).    
Einen Github Account sollten sie ebenfalls anlegen.   
Git müssen sie ebenfalls installieren. Zur Installation ziehen
sie das Internet zu Raten.     
Unter MacOS ist für solche Utilities die Installation von homebrew (https://brew.sh) sehr zu empfehlen.

### Spreadsheets

Auf Windows und MacOS sollten sie auch Microsoft Excel und Microsoft Word und/oder LibreOffice (https://www.libreoffice.org) installiert haben, auf Linux LibreOffice.

	
	
