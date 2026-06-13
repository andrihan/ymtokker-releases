<h1 align="center">YMTokker Downloader</h1>

<p align="center">
  Téléchargeur vidéo de bureau pour Linux et Windows — YouTube, playlists, ~1000 sites, torrents.
</p>

<p align="center">
  <a href="https://github.com/andrihan/ymtokker-releases/releases/latest"><img alt="Dernière version" src="https://img.shields.io/github/v/release/andrihan/ymtokker-releases?label=version&sort=semver"></a>
  <a href="https://github.com/andrihan/ymtokker-releases/releases"><img alt="Téléchargements" src="https://img.shields.io/github/downloads/andrihan/ymtokker-releases/total?label=t%C3%A9l%C3%A9chargements"></a>
  <img alt="Plateformes" src="https://img.shields.io/badge/plateformes-Linux%20%7C%20Windows-informational">
</p>

---

Application de bureau pour récupérer des vidéos et de l'audio depuis le web : choix de la
qualité, téléchargements en parallèle avec file d'attente, **pause / reprise**, reprise
automatique après coupure, extraction **MP3** (tags + pochette), sous-titres `.srt`, recherche
intégrée, et téléchargement de **torrents** et liens **magnet** — le tout dans une interface
unique, en **français, anglais et malgache**.

Ce dépôt ne contient **que les binaires publiés**. Récupérez la dernière version sur la
[**page des releases**](https://github.com/andrihan/ymtokker-releases/releases/latest).

## Installation

### Linux (Debian / Ubuntu)

```bash
sudo apt install ./ymtokker-downloader_<version>_amd64.deb
```

`apt` installe automatiquement les dépendances graphiques. L'application apparaît ensuite
dans le menu, et les commandes `ydown` (CLI) / `ydown-gui` sont disponibles dans le `PATH`.

### Windows

Téléchargez `ymtokker-downloader-<version>.exe` et lancez-le — aucune installation requise.

## Dépendances

| Outil | Requis pour | Linux | Windows |
|-------|-------------|-------|---------|
| **ffmpeg** | fusion HD (DASH) et conversion MP3 | `sudo apt install ffmpeg` | placer `ffmpeg.exe` à côté de l'`.exe` ou dans le `PATH` |
| **yt-dlp** | sites autres que YouTube | `sudo apt install yt-dlp` | placer `yt-dlp.exe` à côté de l'`.exe` ou dans le `PATH` |
| **VLC** *(optionnel)* | lecture en streaming (« Regarder ») | `sudo apt install vlc` | installation standard |

> Sur Windows, l'application cherche `ffmpeg.exe` et `yt-dlp.exe` **dans son propre dossier** :
> il suffit de les déposer à côté de `ymtokker-downloader.exe`.

## Fonctionnalités

- **Sources** : YouTube (moteur natif), ~1000 sites via yt-dlp (Facebook, Instagram, TikTok,
  Vimeo, Dailymotion…), détection des vidéos d'une page, **torrents / magnets** (client intégré).
- **Qualités** : de 360p à la meilleure disponible, ou **audio MP3** (tags ID3 + pochette).
- **Playlists** : sélection des vidéos à cocher, qualité commune, taille totale estimée.
- **Téléchargements** : plusieurs en parallèle, file d'attente configurable, **pause / reprise / arrêt**,
  reprise automatique après fermeture ou coupure réseau.
- **Sous-titres** : export `.srt` dans la langue choisie.
- **Lecture** : « Regarder » lit le flux en streaming sans télécharger.
- **Confort** : recherche YouTube intégrée, ouverture du dossier en un clic, thème clair / sombre,
  interface **FR / EN / MG**.

## Mises à jour

L'application vérifie les nouvelles versions au démarrage. Lorsqu'une mise à jour est
disponible, elle peut être **téléchargée et installée en un clic** depuis l'application
(sous Linux, via une demande de mot de passe administrateur).

## Avertissement

Outil destiné au téléchargement de contenus que vous avez le droit d'enregistrer (vidéos
personnelles, contenus libres, ISO, etc.). Respectez les conditions d'utilisation des
plateformes et la législation sur le droit d'auteur en vigueur.

## Licence

Distribué gratuitement. Voir le dépôt principal pour les détails de licence.
