# BoardgameGeek Metadata Source Plugin for Calibre

## Overview

This is a plugin for [Calibre](https://calibre-ebook.com/) that searches for book metadata from [Boardgamegeek](https://www.boardgamegeek.com/). This is a fork of the RPGGeek plugin developed by the excellent Erik Levin! (Thanks Erik!)

## Develop

Requirements:
- Python
- Calibre

I suggest working directly from Erik's base plugin rather than doing a fork of this one

```
git clone https://github.com/kovidgoyal/calibre.git

git clone https://github.com/ErikLevin/calibre_rpggeek_plugin.git
cd calibre_rpggeek_plugin
python -m venv .venv
.venv/Scripts/activate
pip install -r requirements.txt
```

In .venv/Lib/site-packages, create a file Calibre.pth.

In that file, enter {path to where you cloned Calibre}/src.

### Test

```
calibre-customize -b .
calibre-debug -e test.py
```
