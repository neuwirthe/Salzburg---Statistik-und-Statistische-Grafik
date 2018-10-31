# Statistik und Statistische Grafik

### LV Nr 	405.365


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
	* Wenn die Installatoion fertig ist starten sie `RStudio` vom Start Menu.
	* Nachdem RStudio läuft erscheint ein Icon im Taskbar. Klicken sie aif das Icon unf führen sie `Pin to Taskbar` aus.

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
"ggthemes",
"ggThemeAssist",
"ggplot2movies",
"ggmap",
"ggrepel",
"ggwordcloud",
"scales",
"sf",
"maptools",
"rgeos",
"pracma",
"readxl",
"writexl",
"Dykstra",
"quadprog",
"devtools"
)

install.packages(pkgs_to_install)
```

und führen sie diesen Code aus (dazu einfach Return drücken)

#### Github


Das Herunterladen der Materialien geht einfacher, wenn sie auch noch einen Github-Account (auf https://github.com) anlegen.

Das geht  auf dieser Seite: https://github.com/join?source=header-home

Wählen sie bei der Registrierung den `Free Plan` aus.

Außerdem müssen sie `git` von hier https://github.com/git-for-windows/git/releases/download/v2.19.1.windows.1/Git-2.19.1-64-bit.exe installieren.

Führen sie dann noch (in einem Command-Fenster) folgenden Befehl aus:   
`git config --global credential.helper wincred`




	
	
	
