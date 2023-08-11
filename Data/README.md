# Weighted network data sets

* [Network data sets](http://vladowiki.fmf.uni-lj.si/doku.php?id=vlado:ed:ss:dat)
* [Sources](https://github.com/BS-SNS/Public/tree/main/data)


| Network | Nodes    | Weight    |  Sizes | Description |
| :---         |     :---       |     :---       |     :---       |      :---:   |
| [Trade1985](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985.net)   | country    | export USD    | n = 192, m = 12743    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [Trade1985cn](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985cn.net)   | country    | export USD    | n = 192, m = 12743      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [WTyears](https://raw.githubusercontent.com/bavla/wNets/main/Data/WTyears.zip)   | country    | export USD    | n = 238, y = 27    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |
| [WTtime](https://raw.githubusercontent.com/bavla/wNets/main/Data/WRtime.zip)   | country    | export USD    | n = 238, y = 27      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |

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
