Si vous utilisez un logiciel qui lit les .NFO (Jellyfin, Kodi...), pas besoin de lire le tuto Plex mais je vous invite à lire les remarques.

I) Petit tutoriel pour avoir nos productions sur Plex dans de meilleures conditions :

1) Installez Plex Media Server
2) Dézippez tout le contenu du .zip
3) Mettez "XBMCnfoTVImporter.bundle" dans %localappdata%\Plex Media Server\Plug-ins, si vous avez un NAS ou autre système d'exploitation, il va falloir fouiller un peu, ça devrait être facile à trouver !
3.1) Voici où peut ce trouver votre dossier Plug-in selon le système où est installé votre Plex : 
* '%LOCALAPPDATA%\Plex Media Server\'                                        # Windows Vista/7/8
* '%USERPROFILE%\Local Settings\Application Data\Plex Media Server\'         # Windows XP, 2003, Home Server
* '$HOME/Library/Application Support/Plex Media Server/'                     # Mac OS
* '$PLEX_HOME/Library/Application Support/Plex Media Server/',               # Linux
* '/var/lib/plexmediaserver/Library/Application Support/Plex Media Server/', # Debian,Fedora,CentOS,Ubuntu
* '/usr/local/plexdata/Plex Media Server/',                                  # FreeBSD
* '/usr/pbi/plexmediaserver-amd64/plexdata/Plex Media Server/',              # FreeNAS
* '${JAIL_ROOT}/var/db/plexdata/Plex Media Server/',                         # FreeNAS
* '/c/.plex/Library/Application Support/Plex Media Server/',                 # ReadyNAS
* '/share/MD0_DATA/.qpkg/PlexMediaServer/Library/Plex Media Server/',        # QNAP
* '/volume1/Plex/Library/Application Support/Plex Media Server/',            # Synology, Asustor
* '/raid0/data/module/Plex/sys/Plex Media Server/',                          # Thecus
* '/raid0/data/PLEX_CONFIG/Plex Media Server/'                               # Thecus Plex community
4) Redémarrez Plex Media Server
4.5) Si vous avez un environnement Windows ayant accès à Plex en local téléchargez Plex-Config du dossier Setup et suivez les instructions. Vous pouvez vous arrêtez ici.

5) Créez une nouvelle bibliothèque ayant pour contenu "Séries" (TV Shows) et pour agent "XBMCnfoTVImporter"
6) Allez dans les paramètres de Plex (Clé à molette), dans agents, puis séries et enfin XBMCnfoTVImporter, cochez local media assets (TV)

7) Faites en sorte d'avoir les films bien rangés avec les affiches et NFO (lire remarques ou utilisez l’utilitaire Fankai disponible sous Windows si vous avez accès à vos dossiers de films).

8) Faites un scan de votre bibliothèque (les trois petits points en haut à gauche) à chaque nouveauté.
9) Au cas où les films n'auraient pas les bonnes affiches, pensez à rafraîchir les métadonnées, faites "corriger l'association" au cas où la série serait mal associée.
10) Vous êtes fin prêt à lire notre contenu !


II) Quelques remarques :

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
Laissez la magie opérer et tout sera reconnu, voici la liste pour les plus curieux :


- Jojo's Bizarre Adventure (Diamond is Unbreakable) : remplacer le film 6 par "[Livaï] Jojo’s Bizarre Adventure Diamond is Unbreakable Henshū 06 - Jeudi Quinze Juillet - 1080p.VOSTFR.x264"
- One Piece (Saison 3) : remplacer le film 22 par "One Piece Yabai S03E22 [Mixouille]"
- Monster (Film 6) : retirer "511" -> "Monster Kaï - 02 - Kinderheim"

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
