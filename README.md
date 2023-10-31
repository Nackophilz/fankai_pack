<br/>
<p align="center">
  <h3 align="center">Fankai-Pack</h3>

  <p align="center">
    Regroupement des Pack NFO et des différentes version de l'Utilitire de @ElPouki
    <br/>
    <br/>
    <a href="https://github.com/ElPouki/fankai_pack/issues">Report Bug</a>
    .
  </p>
</p>

![Downloads](https://img.shields.io/github/downloads/ElPouki/fankai_pack/total) ![Contributors](https://img.shields.io/github/contributors/ElPouki/fankai_pack?color=dark-green) ![Issues](https://img.shields.io/github/issues/ElPouki/fankai_pack) ![License](https://img.shields.io/github/license/ElPouki/fankai_pack) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

Ce projet a été créé afin de faciliter la reconnaissance des différents Films Kai par nos médias server préférer

## Getting Started

Si vous utilisez un logiciel qui lit les .NFO (Jellyfin, Kodi...), pas besoin de lire le tuto Plex mais je vous invite à lire les remarques.

### Prerequisites

Un MediaServer (Plex,Jellyfin...etc.) fonctionnel 
Avoir télécharger le plugin XBMC dispo dans ce repo
Du temps

### Installation

1) Mettez "XBMCnfoTVImporter.bundle" :

Voici où peut se trouver votre dossier Plug-in selon le système sur lequel est installé votre Plex : 
- Windows Vista/7/8:
'%LOCALAPPDATA%\Plex Media Server\Plug-ins'
- macOS:
'$HOME/Library/Application Support/Plex Media Server/Plug-ins'
- Linux:
'$PLEX_HOME/Library/Application Support/Plex Media Server/Plug-ins'
- Debian,Fedora,CentOS,Ubuntu:
'/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/Plug-ins'
- FreeBSD:
'/usr/local/plexdata/Plex Media Server/Plug-ins'
- FreeNAS:
'${JAIL_ROOT}/var/db/plexdata/Plex Media Server/Plug-ins'
'/usr/pbi/plexmediaserver-amd64/plexdata/Plex Media Server/Plug-ins'
- QNAP:
'/share/MD0_DATA/.qpkg/PlexMediaServer/Library/Plex Media Server/Plug-ins'
- Synology, Asustor:
'/volume1/Plex/Library/Application Support/Plex Media Server/Plug-ins'
- Thecus:
'/raid0/data/module/Plex/sys/Plex Media Server/Plug-ins'
- Thecus Plex community:
'/raid0/data/PLEX_CONFIG/Plex Media Server/Plug-ins'

2) Redémarrez Plex Media Server
2.5) Vous pouvez utiliser le Fankai-Config selon votre système à partir d'ici puis l'utilitaire principal, si vous souhaitez continuer manuellement c'est juste en dessous.

3) Créez une nouvelle bibliothèque ayant pour contenu "Séries" (TV Shows) et pour agent "XBMCnfoTVImporter"
4) Allez dans les paramètres de Plex (Clé à molette), dans agents, puis séries et enfin XBMCnfoTVImporter, cochez local media assets (TV)

5) Faites en sorte d'avoir les films bien rangés avec les affiches et NFO (lire remarques ou utilisez l’utilitaire Fankai disponible sous Windows si vous avez accès à vos dossiers de films).

6) Faites un scan de votre bibliothèque (les trois petits points en haut à gauche) à chaque nouveauté.
7) Au cas où les films n'auraient pas les bonnes affiches, pensez à rafraîchir les métadonnées, faites "corriger l'association" au cas où la série serait mal associée.
8) Vous êtes fin prêt à lire notre contenu !




## Usage

1) Vous trouverez plusieurs saisons quelques fois qui ne seront pas renommées au sein de Plex, malheureusement le logiciel ne gère pas cette "automatisation", mais grâce à @ElPouki, un script vous permet de faire l'automatisation ! 
Télécharger puis ouvrez simplement "Fankai.exe" dans le dossier "Setup" si il n'est pas déjà présent chez vous et suivez les instructions.

2) Pour toutes suggestions, corrections d'erreurs ou autre, n'hésitez pas à en faire part dans notre Discord (linktr.ee/FanKai) !
Le pack est sujet à avoir des mises à jour à chaque sortie de film ou pour des corrections/ajouts, n'hésitez pas à remplacer les fichiers actuels en conséquence (ou utilisez le choix Fankai-Pack de l’utilitaire qui gère les mises à jour et ajout de nouveaux packs pour vous).

3) Voici la liste de ce qui a été fait pour construire les packs: 

Affiche de la série, affiche de chaque saison, distribution (les voix japonaises), année originale de diffusion, genres du titre, description, studio (nom du kaieur + Fan-Kai), affiche de fond (fanart/background).

Titres de films, date de sortie (si elle est connue), résumé du premier épisode figurant dans le Kaï, guide de l'épisode (épisodes + chapitres si disponible), affiches de films.

Certains films non sortis sont déjà dispos en .NFO, c'est que ces films sont déjà répertoriés sur le fandom.

4) Les résumés et descriptions sont pris sur TVDB ou TMDB, ils ne sont des fois pas dispos en français, je les ai donc traduits, si vous pensez qu'une faute s'est glissée, vous pouvez la faire remonter, elle sera corrigée au plus vite.
Chaque film n'a pas forcément été relu, si des fautes hors traduction se sont glissées, merci d'en faire part. (par exemple dans death note, des "Raito" au lieu de "Light" s'étaient glissés)

5) Afin que je n'ai pas à tout télécharger, vous verrez si vous fouillez que les .NFO disent que la vidéo fait du 640*480, j'ai en effet copié/collé des épisodes de 2 Mo afin de pouvoir les faire reconnaître dans mon logiciel de NFO (TinyMediaManager)
Après de multiples vérifications, il s'avère que ça n'impacte en rien ce qui est affiché sur Plex/autre tant que vous avez le bon film.

6) N'ayant pas vu tous les kai disponibles, j'ai dû mettre ce qu'il fallait sans checker, si vous trouvez une erreur, quelque chose qui semble faux comme l'affiche de saison par exemple (selon votre connaissance), n'hésitez pas à en faire part également.

7) Certains kai doivent être renommés ! En effet, ils peinent à être reconnus par Plex (par exemple), je vous invite donc à utiliser le choix"Fankai-Films" de l’utilitaire qui permet de renommer de manière automatique tous vos fichiers.
Laissez la magie opérer et tout sera reconnu.

C'est également le cas des chiffres qui n'ont pas de 0 devant eux, un renommage particulier a été fait sur les films 1 à 9 de chacun sur la liste, utilisez bien le script "ChangeName" trouvable dans "Setup" et ce sera bon, au cas où, voici la liste :

- Enfer et Paradis
- Fullmetal Alchemist
- Haikyu
- Hokuto no Ken (à renommer entièrement selon les .png/nfo)
- Jojo's Bizarre Adventure (chaque partie)
- Kuroko no Basket (saison 2)
- Lastman
- My Hero Academia
- Reborn
- Seven Deadly Sins
- Shiki
- Slam Dunk
- Yu Yu Hakusho



## Authors

* **ElPouki** - *Initiator* - [ElPouki]() - **
* **Hikano** - *Initiator* - [Hikano]() - **