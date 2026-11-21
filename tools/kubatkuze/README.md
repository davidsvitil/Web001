# Aktualizace dat
```bash
python3 tools/kubatkuze/fetch_pages.py urls.txt raw/pages
python3 tools/kubatkuze/parse_shop.py shoptet raw/pages raw/parsed.json
python3 tools/kubatkuze/build_catalog.py raw/parsed.json kubatkuze tools/kubatkuze/config.json
HERO_HOLES=1 python3 tools/kubatkuze/make_hero.py kubatkuze <id produktu> ...
```
Potřeba: Python 3, Pillow, BeautifulSoup4, lxml, curl.
