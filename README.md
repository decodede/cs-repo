<div align="center">

# 🍪 Few Cookies

**Ten CloudStream 3 plugins. Paste one link into CloudStream and you're done.**

[⬇️ Tap to install in CloudStream](https://self-similarity.github.io/http-protocol-redirector?r=cloudstreamrepo://github.com/decodede/cs-repo/raw/main/repo.json)

```
https://raw.githubusercontent.com/decodede/cs-repo/main/repo.json
```

</div>

---

## Install

**In the app:** CloudStream → _Settings_ → _Add repository_ → paste the link above.

**On a TV/remote:** open the first link on a phone, it hands the repository to CloudStream.

Then pick whichever plugins you want in _Settings_ → _Extensions_.

## What's in this repo

This is the **distribution** repo. It is generated — every file here is rebuilt and pushed
automatically, so don't edit anything by hand.

```
plugins.json    the list of available plugins and their download URLs
repo.json       the repository manifest CloudStream reads when you add it
*.cs3           the plugins themselves (a ZIP of manifest.json + classes.dex)
icons/          repository and per-plugin icons
```

Source code lives in the private `decodede/cs-code`. Everything a client has to download is
here, because `raw.githubusercontent.com` returns `404` for private repositories and CloudStream
downloads anonymously.

## Plugins

| Plugin    | Version | Provides                                                     |
| --------- | ------- | ------------------------------------------------------------ |
| FindDrama | v1      | Short dramas in one place                                    |
| kimoitv   | v1      | Hollywood, Korean, Chinese, Japanese movies & series         |
| Kisskh    | v6      | Asian dramas, Hollywood, anime, movies with subtitles        |
| NunoDrama | v1      | Short drama providers as catalogues, EN/ID                   |
| ReelFren  | v1      | Every ReelFren site as its own provider                      |
| Rulz      | v5      | Telugu movies and dubbed cinema                              |
| Screen    | v2      | Telugu movies, post-OTT in HD                                |
| Stremio   | v4      | Plays anything your Stremio addons can find                  |
| Wap       | v2      | Telugu movies, series, Hollywood dubbed                      |
| Wood      | v11     | Telugu, Hindi, English, Tamil, Malayalam movies & web series |

Plugins update themselves from this repo, so CloudStream picks up new versions without you
doing anything.

## Troubleshooting

**The repository shows as empty.** Make sure you added `repo.json`, not `plugins.json` —
`repo.json` is the manifest, and it is what points CloudStream at the plugin list.

**A plugin has no icon.** Icons are served from here, not from the source repo, because the
source repo is private. If an icon is blank the file is missing from `icons/`.

**A download fails.** Check that `plugins.json` points at
`raw.githubusercontent.com/decodede/cs-repo/main/`. Any other host is stale.

## Disclaimer

For educational purposes only. You are responsible for ensuring your use complies with the
laws and regulations of your jurisdiction.
