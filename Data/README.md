# Weighted network data sets

* [Network data sets](https://github.com/bavla/Nets/tree/master/data)
* [Network data sets](http://vladowiki.fmf.uni-lj.si/doku.php?id=vlado:ed:ss:dat)
* [Sources](https://github.com/BS-SNS/Public/tree/main/data)

## Weighted networks

| Network | Nodes | Edges | Arcs | Weight | Description |
| :---         |     :---       |     :---       |     :---       |     :---       |      :---:   |
| [EAT](http://vlado.fmf.uni-lj.si/pub/networks/data/dic/eat/Eat.htm)   | ?    | ? | ? | frequency     | [str](https://github.com/bavla/ibm3m/blob/master/data/str/VisTest.md)     |
| [Football](http://vlado.fmf.uni-lj.si/pub/networks/data/sport/football.htm)   | ?    | ? | ? | frequency     | [str](https://github.com/bavla/ibm3m/blob/master/data/str/VisTest.md)     |


| Network | Nodes    | Weight    |  Sizes | Description |
| :---         |     :---       |     :---       |     :---       |      :---:   |
| [Trade1985](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985.net)   | country    | export USD    | n = 192, m = 12743    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [Trade1985cn](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985cn.net)   | country    | export USD    | n = 192, m = 12743      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [WTyears](https://raw.githubusercontent.com/bavla/wNets/main/Data/WTyears.zip)   | country    | export USD    | n = 238, y = 27    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |
| [WTtime](https://raw.githubusercontent.com/bavla/wNets/main/Data/WRtime.zip)   | country    | export USD    | n = 238, y = 27      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |
| [StarWars](https://raw.githubusercontent.com/bavla/wNets/main/Data/StarWarsE.net)   | SW character  | # coaapearances    | n = 111, m = 555      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#starwars)     |

## Trade1985

Data set used in the paper:
Jiang, X. R., Yang, Y. C., Wang, S. L.: Trade Network Dataset Development in 227 Countries and Regions (1985-2015). 
   Journal of Global Change Data & Discovery,2019.3(3):227-233. DOI: 10.3974/geodp.2019.03.02
 https://www.geodoi.ac.cn/WebEn/doi.aspx?ID=1230&paperID=a467897d-0a56-41dc-85d3-dfc9b030f7a9
 
Original source: United Nations Conference on Trade and Development（UN Comtrade International Trade Statistics Database: https://unctad.org/en/Pages/Statistics.aspx).

Transformed into Pajek format by Vladimir Batagelj.

## US 2016

[data](https://github.com/bavla/cluRC/tree/master/data); [wiki](http://vladowiki.fmf.uni-lj.si/doku.php?id=pro:relc:us)

## WT

Aggregated world trade data from [BACI / CEPII](http://www.cepii.fr/CEPII/en/bdd_modele/bdd_modele_item.asp?id=37). Weight is the trade flow (in thousands current USD). Transformed into Pajek format by Vladimir Batagelj, Fri Aug 11, 2023.

WTyears contains a network for each year; WTtimes contains a single temporal network for all years. The countries are labeled using ISO 2-character codes.
ISO3.nam contains ISO 3-character codes, and countries.nam the long names.

## StarWars 

(undirected with loops)
**nodes:** characters from the Star Wars universe; **links:** coappearance; **weight:** Number of scenes in which the character appears / both characters appear together.<br />
Transformed into Pajek format by Vladimir Batagelj, Sun Feb 9, 2025.

The Star Wars Network dataset provides a unique opportunity for social network analysis using characters from the Star Wars universe. The Kaggle dataset comprises two CSV files:<br />starwars-characters.csv: Contains a list of characters with the following columns:
- number: Unique identifier for each character.
- name: The name of the character.
- scenes: Number of scenes in which the character appears.

starwars-links.csv: Captures the interactions between characters with the following columns:
- character1: Name or ID of the first character.
- character2: Name or ID of the second character.
- scenes: Number of scenes in which both characters appear together.

- https://www.kaggle.com/datasets/mexwell/star-wars-network/versions/1
- https://github.com/chatox/networks-science-course/tree/master/practicum/data/starwars
- https://github.com/evelinag/star-wars-network-data


