

Titel:      Dokumentattion von Git/Github Repository
Date:       04-11-2022
Author:     Reza Motahari
Keywords:   Git, Github, Linux


# Git Repository lokal erstellen

## Projekt Umgebung vorbereiten

##### SSH Schluessel Key erstellen

	ssh-keygen

##### Kopieren PublicKey in GitHub
		
		cat .ssh/id_rsa.pub

####### Ueberprufen die Verbindung mit GitHub

		ssh -T git@github.com
		git remote add origin git@github.com:ingeniebrio77/Arcolinux_git.git
		

#### Erstellen Sie ein Vezeichnis mit dem Name Projekt1

    cd
    mkdir Projekt1

#### Dateien und Verzeichnisse fuer das Projekt "Statische Webseite"

    touch index.html style.css backend.py 
    mkdir Secret
    cd Secret
    touch Geheimnisse.txt
    cd ..
    mkdir Bilder
    cd Bilder
    touch Bild1.jpg Bild2.jpg Bild3.jpg Bild1.png Bild2.png
    cd ..
    touch .gitignore

#### Falls dass Sie sensibel Daten Verstecken wollen, schreiben Sie welche in .gitignore File und speicher die Aenderungen

    nano .gitignore

Code-Blocke

    Secret/
    Bilder/*.png

#### Git Umgebung vorbereiten

    git config --global user.name "Name Nachname"
    git config --global user.email "valid-email"

#### git Kontrollversionierung initialisiren

    git init

#### From Working Area nach Stagin Area nach Repositoty

    git status
    git add -A
    git commit -m "Erstes Commit"
    git status

###### Lokal Repository "Push" zum GitHub
    git push -u origin master

###### für upload 
        git push

######  für download in lokal 
	git pull

######  nach any Änderung 
    git status
    git add -A
    git commit -m "Erstes Commit"
    git status
    git push

#####    
    
