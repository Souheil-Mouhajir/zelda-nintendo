# Does Zelda sell the console?

This repository holds the mid term project for **DATS 2102, Data Visualization for Data Science** (Professor Junjun Yin, The George Washington University, fall 2026), by Souheil Mouhajir.

The project measures how far The Legend of Zelda reaches into the audience of each Nintendo console. It joins VGChartz sales estimates for 16,692 titles (to December 2016), Nintendo's official hardware and software figures (to 30 June 2026) and the Metacritic record of the series. The median Zelda title sold 2.9 million copies, against 170,000 for the median title in the file. Measured per 100 consoles sold, Zelda reaches 46 on the Switch and 5 on the DS. Eleven figures drawn in matplotlib present the analysis.

## Contents

| Path | What it is |
|---|---|
| `zelda_nintendo.ipynb` | The notebook with all code, outputs and text |
| `zelda_nintendo.html` | The Quarto render of the notebook, self contained |
| `reflection.docx` | The reflective essay (318 words, double spaced) |
| `data/raw/` | The four input CSV files |
| `style.css`, `banner.html`, `daynight.html` | Page style, title banner and the clock based light and dark start |
| `fonts/` | Fira Sans (SIL Open Font Licence, see `fonts/OFL.txt`) and the Triforce title font |
| `images/` | The banner image |

## Reproducing the analysis

The notebook was run with Python 3.13 and rendered with Quarto 1.10.

```
pip install -r requirements.txt
jupyter nbconvert --to notebook --execute --inplace zelda_nintendo.ipynb
quarto render zelda_nintendo.ipynb --to html
```

All paths in the notebook are relative to the repository root, so it runs from a fresh clone. The bootstrap uses a fixed seed and gives the same intervals on every run.

## Data sources

Kirubi, R. (2016). *Video game sales with ratings* [Data set]. Kaggle. Mirrored at https://github.com/chahelgupta/DEP-videogames-dataset

Nintendo Co., Ltd. (2026a). *Dedicated video game sales units* [Data set]. https://www.nintendo.co.jp/ir/en/finance/hard_soft/index.html

Nintendo Co., Ltd. (2026b). *Top selling title sales units* [Data set]. https://www.nintendo.co.jp/ir/en/finance/software/index.html

The legend of Zelda. (2026). In *Wikipedia*. Retrieved October 22, 2026, from https://en.wikipedia.org/wiki/The_Legend_of_Zelda

List of best-selling Nintendo Switch video games. (2026). In *Wikipedia*. Retrieved October 22, 2026, from https://en.wikipedia.org/wiki/List_of_best-selling_Nintendo_Switch_video_games

## Rights

The text, code and figures are by Souheil Mouhajir. The Hyrule Field banner is from The Legend of Zelda: Breath of the Wild (Nintendo, 2017) and belongs to Nintendo; it is used here for non commercial coursework.
