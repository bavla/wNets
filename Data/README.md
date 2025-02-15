# Weighted network data sets

* [Network data sets](https://github.com/bavla/Nets/tree/master/data)
* [Network data sets](http://vladowiki.fmf.uni-lj.si/doku.php?id=vlado:ed:ss:dat)
* [Sources](https://github.com/BS-SNS/Public/tree/main/data)

## Weighted networks






| Network | Nodes    | Weight    |  Sizes | Description |
| :---         |     :---       |     :---       |     :---       |      :---:   |
| [EAT](https://raw.githubusercontent.com/bavla/wNets/main/Data/EATnewSR.net)   | word    | assoc. frequency | n =  23219, mA =325589, m0 = 564   |  [desc](http://vlado.fmf.uni-lj.si/pub/networks/data/dic/eat/Eat.htm)     |
| [Football](https://raw.githubusercontent.com/bavla/wNets/main/Data/football.net)   | country    | # players | n = 35      | [desc](http://vlado.fmf.uni-lj.si/pub/networks/data/sport/football.htm)     |
| [Trade1985](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985.net)   | country    | export USD    | n = 192, m = 12743    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [Trade1985cn](https://raw.githubusercontent.com/bavla/wNets/main/Data/Trade1985cn.net)   | country    | export USD    | n = 192, m = 12743      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#trade1985)     |
| [WTyears](https://raw.githubusercontent.com/bavla/wNets/main/Data/WTyears.zip)   | country    | export USD    | n = 238, y = 27    | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |
| [WTtime](https://raw.githubusercontent.com/bavla/wNets/main/Data/WRtime.zip)   | country    | export USD    | n = 238, y = 27      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#WT)     |
| [StarWars](https://raw.githubusercontent.com/bavla/wNets/main/Data/StarWarsE.net)   | SW character  | # co-apearances    | n = 111, m = 555      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#starwars)     |
| [StarWarsRT](https://raw.githubusercontent.com/bavla/wNets/main/Data/StarWars.paj)   | SW character  | # co-apearances    | n = 113, m = 3827, T = 1-7, r = 3      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#starwarsRT)     |
| [Spotify 10](https://raw.githubusercontent.com/bavla/wNets/main/Data/3000_genres_c10.net)   | music genre  | dissimilarity    | n = 3000, mA = 30000      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#Spotify)     |
| [Spotify top 2022](https://raw.githubusercontent.com/bavla/wNets/main/Data/SpotifyTop22.paj)   | artist  | # collaborations    | n = 309, m = 2445      | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#Spotify22)     |
| [Erasmus 14](https://raw.githubusercontent.com/bavla/wNets/main/Data/ErasmusFlows.net)   | country  | # visitors    | n = 35, mA = 1223     | [desc](https://github.com/bavla/wNets/blob/main/Data/README.md#Erasmus14)     |





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

The Kaggle dataset comprises two CSV files:<br />starwars-characters.csv: Contains a list of characters with the following columns:
- number: Unique identifier for each character.
- name: The name of the character.
- scenes: Number of scenes in which the character appears.

starwars-links.csv: Captures the interactions between characters with the following columns:
- character1: Name or ID of the first character.
- character2: Name or ID of the second character.
- scenes: Number of scenes in which both characters appear together.

Sources
- https://www.kaggle.com/datasets/mexwell/star-wars-network/versions/1
- https://github.com/chatox/networks-science-course/tree/master/practicum/data/starwars
- https://github.com/evelinag/star-wars-network-data

## StarWarsRT

Star Wars Network / undirected, temporal, multi-relational

The creation of the Kaggle Star Wars data is described at
[GitHub/chatox](https://github.com/chatox/networks-science-course/tree/master/practicum/data/starwars) where we learn that it is based on the data collected by [Evelina Gabasova](https://github.com/evelinag/star-wars-network-data).

Evelina Gabasova. (2016). Star Wars social network (Version 1.0.1) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.1411479

Evelina's data are more detailed - they determine a temporal multi-relational weighted network.
7 episodes determine the time 1-7; time = 8 corresponds to all 7 episodes merged. There are 3 relations: 1-mentions, 2-interactions, and 3-interactions-allCharacters.

weight: Number of scenes in which both characters appear together; time 1-7, time=8 merged<br />
partitions: Number of scenes in which the character appears (i3 - interactions in the episode 3)

Transformed into Pajek format by Vladimir Batagelj (uvFac2Pajek Mon Feb 10 05:04:52 2025)  from  https://github.com/evelinag/star-wars-network-data

In Pajek, all created Pajek files (network and partitions) were combined into a single Pajek project file ''StarWars.paj''. We manually changed Arcs -> Edges, added some metadata, and made some cleaning.

In Pajek we can now extract subnetworks of our interests.

## Spotify

Spotify's top 3000 music genres - Network / closest 10 neighbors

From [Kaggle](https://www.kaggle.com/datasets/georgeggcoco/closeness-of-music-genres/versions/1) (2023-08-04T13:27:45.393).

This dataset was created based on the work done by [Glenn McDonald](https://furia.com)  over on his website [Every Noise at Once](https://everynoise.com/everynoise1d.cgi). 
George G Coco created and used this dataset for an [interactive network of music genres](https://chartingsounds.streamlit.app).

The dataset includes 3000 music genres in a square grid of dimensions `3000 x 3000` which essentially works as a Heat-Map:
  - Rows and Column names are the names of music genres (by popularity, desc)
  - The values are an abstract 'distance'. A small value means those genres are closely related. A big value means those genres are not related.
  - If you're interested in how exactly this value was calculated, you can read about it in the Provenance section of this dataset.

The numerical values are obtained by multiplying the rank (list index) of two genres on each other's lists. For example: If we have genre 'A' and genre 'B':
  - We store the rank (index) value of 'B' in the list rooted on 'A'
  - We store the rank (index) value of 'A' in the list rooted on 'B'
  - We multiply these two values. The result is the distance.

Converted into Pajek format by Vladimir Batagelj (mat2Pajek Mon Feb 10 15:33:27 2025). 

The network is directed. For most applications convert it to an undirected network first.

The complete network [3000_genres](https://raw.githubusercontent.com/bavla/wNets/main/Data/3000_genres.7z)(7z) is quite large. The corresponding [matrix](https://raw.githubusercontent.com/bavla/wNets/main/Data/3000_genres.rds) is provided in R data format.

## Spotify22

Musical collaborations between top artists in 2022

Based on the data set posted by Terenci Claramunt on [Kaggle](https://www.kaggle.com/datasets/terencicp/musical-collaborations-between-top-artists-in-2022).
TC used this dataset to create an [interactive network plot](https://public.flourish.studio/story/2151064/) of the collaborations between the top artists on Spotify in 2022.
To obtain the data necessary TC extracted a list of the most popular Spotify artists from [Sveta151's dataset](https://www.kaggle.com/datasets/sveta151/spotify-top-chart-songs-2022).

Afterward, TC used MusicBrainz API to get a list of songs for each artist, including the artists who worked on each song. Then he calculated the number of collaborations for each pair of artists and split the data into a table of artists and a table of collaborations between artists.

Converted into Pajek format by Vladimir Batagelj (uvFac2Pajek Tue Feb 11 07:15:17 2025).

Besides the collaboration network, the file SpotifyTop22.paj contains also the two-mode (Artists, Genres) network, 2 partitions (type.clu: Gender of the artist or Band, country.clu: Country of the artist), and 2 vectors (coSongs.vec: Number of songs in which the artist collaborated, coArtists.vec: Number of artists the artist collaborated with).

## Erasmus14

Erasmus learning mobility flows between countries since 2014

Data were downloaded as a CSV file from the interactive diagram at the bottom of the page  [Data visualisation on learning mobility projects](https://erasmus-plus.ec.europa.eu/resources-and-tools/factsheets-statistics-evaluations/statistics/data/learning-mobility-projects).

Nodes are countries. The weight of an arc (from, to) counts the number of participants from the country from that visited the country to. [ISO 2-character short names](https://raw.githubusercontent.com/bavla/wNets/main/Data/ErasmusFlowsISO.nam) are available.


Converted into Pajek format by Vladimir Batagelj (uvFac2Pajek Wed Feb 12 06:19:43 2025)

<hr>

[Network data sets](https://github.com/bavla/Nets/tree/master/data/README.md)

