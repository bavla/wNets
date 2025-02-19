# Erasmus

At the bottom of the Erasmus+ page 
[Data visualization on learning mobility projects](https://erasmus-plus.ec.europa.eu/resources-and-tools/factsheets-statistics-evaluations/statistics/data/learning-mobility-projects), the "Learning mobility flows since 2014" chart can be found. The interactive chart shows mobility flows between countries since 2014. It also provides an option to download the network data.

The network data were transformed into Pajek network files. 
Nodes are countries. The weight of an arc (from, to) counts the number of participants from the country from that visited the country to. Besides the network file [Erasmus 14](https://raw.githubusercontent.com/bavla/wNets/main/Data/ErasmusFlows.net) the file with 2 character country codes [ISO 2-character short names](https://raw.githubusercontent.com/bavla/wNets/main/Data/ErasmusFlowsISO.nam) and a vector of [total population for each country](https://raw.githubusercontent.com/bavla/wNets/refs/heads/main/Data/PopTotal.vec) are available.
