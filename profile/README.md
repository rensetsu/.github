# Welcome to Rensetsu!

Rensetsu is a project that aims to map several shows, movies, and books databases into one relation entry!

This project was inspired by [anime-offline-database][aod] and [arm], but with a broader scope that
encompasses not only anime but also other forms of media such as movies and books while keeping the database
licensed under MIT and CC0 to ensure open access and collaboration among users and developers alike. Our goal
is to create a comprehensive database that allows users to explore and discover various shows, movies, and
books, all in one centralized location.

## Supported Site

Unlike other competitors, we offered a lot of sites to be mapped into

> [!NOTE]
>
> The following table is not fixed and some sites may removed or added.

|   |   |   |   |   |   |
| :-: | :-: | :-: | :-: | :-: | :-: |
| allcinema | AniBrain.ai | aniDB | AniList | Anime News Network | Anime-Planet |
| Anime-Themes | aniSearch | Annict | Bangumi | Douban | Doujinshi.info |
| IMDb | Kaize | Kitsu | Kinopoisk | Livechart | MangaDex |
| MangaUpdates | MyAnimeList | Nautiljon | Notify.moe | Novel Updates | Otak Otaku |
| SilverYasha DBTI | Shikimori | Syoboicalendar | TMDB | TVDB | Trakt |
| VNDB | Wikidata | | | | |

## Data Sourcing

In Rensetsu, data from a site will be scraped/copied based on its schedule. Some sites may require manual
scraping due to some unique challenge to solve.

Below is a table when and what sites were being scraped, with UTC timezone:

| Monday                       | Tuesday                       | Wednesday | Thursday                   |
| :--------------------------- | :---------------------------- | :-------- | :------------------------- |
| `12:45` [aniDB][adb][^1][^2] | `01:00` [bgm.tv][bgm][^1][^2] |           | `16:30` [AnimeThemes][dmp] |

| Friday                            | Saturday | Sunday                        |
| :-------------------------------- | :------- | :---------------------------- |
| `04:30` [Trakt][trk][^1][^2][^3]  |          | `12:00` [Notify.moe][ntf][^1] |

| Manual                  |
| ----------------------- |
| [SilverYasha DBTI][dmp] |

[^1]: We used publicly available dump to reduce server load to the target site
[^2]: Dump file was provided by 3rd party
[^3]: Currently does not use Rensetsu Media Info data standard.

[aod]: https://github.com/manami-project/anime-offline-database
[arm]: https://github.com/kawaiioverflow/arm
[adb]: https://github.com/rensetsu/db.anidb.rensetsu-diorama
[bgm]: https://github.com/rensetsu/db.bangumi.rensetsu-xingxi
[dmp]: https://github.com/rensetsu/db.rensetsu.public-dump
[trk]: https://github.com/rensetsu/db.trakt.anitrakt
[ntf]: https://github.com/rensetsu/db.notify.rensetsu-mirai
