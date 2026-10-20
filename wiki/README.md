# Wiki source

These files are the source for the [GitHub Wiki](https://github.com/Rocket012/SyncSettings/wiki).

To publish them:

1. Open the Wiki tab on GitHub and create the first page once (any content), so the wiki repository exists.
2. Clone it and copy these files in (without this README):

```
git clone https://github.com/Rocket012/SyncSettings.wiki.git
cp wiki/*.md SyncSettings.wiki/ && rm SyncSettings.wiki/README.md
cd SyncSettings.wiki && git add . && git commit -m "Update wiki" && git push
```

Images are loaded from `assets/` on the `main` branch, so they show up once this branch is merged.
