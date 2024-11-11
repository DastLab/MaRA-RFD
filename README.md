# MARA: Discovery Multi-attribute RFDcs through compact similarity representation of Attributes

## Run parameters

java -jar MaRA.jar input.csv thr(s) -s "," -n "?" -head false -o log_folder -r res_folder -pd true -tl 3600


**input.csv:** CSV file

**thr(s):** numeric value OR space-separated list of numeric values. In the case of a list, each value is associated by position to the respective column of the dataset. The total number of values must be equal to the number of columns in the dataset.

**-s:** CSV separator, DEFAULT:","

**-n:** Char to be considered as NULL value ("blank" OR "" can be used for empty char)

**-head:** If true, the first line of the dataset is considered as header, DEFAULT: true

**-o:** Output log folder, DEFAULT:"log"

**-r:** Output result folder, DEFAULT:false

**-pd:** Parallel discovery

**-tl:** Time limit in seconds



java -jar MaRA.jar input.csv 1 -s "," -n "?" -head false -o log_folder -r res_folder -pd "true" -tl 3600

java -jar MaRA.jar input.csv 1 2 3 4 5 -s ";" -n "blank" -head true -o log_folder -r res_folder -pd "true" -tl 3600 (For a dataset with 5 columns)







## Dataset sources

||Name|Columns|Rows|Source|
| :-------------: | :-------------: | -------------: | -------------: | :------------- |
|1|Restaurant|6|864|[HPI](https://hpi.de/naumann/projects/repeatability/datasets/restaurants-dataset.html)|
|2|Struct|6|169,128|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|3|Abalone|9|4,177|[UCI](https://archive.ics.uci.edu/dataset/1/abalone)|
|4|Nursery|9|12,960|[UCI](https://archive.ics.uci.edu/dataset/76/nursery)|
|5|Gas|9|416,153|[UCI](https://archive.ics.uci.edu/dataset/799/single+elder+home+monitoring+gas+and+position)|
|6|Discs|9|750,000|[HPI](https://hpi.de/naumann/projects/data-integration-data-quality-and-data-cleansing/annealing-standard.html)|
|7|Claim|11|112,500|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|8|Link|11|126,905|[HPI](https://hpi.de/naumann/projects/repeatability/data-profiling/fds.html)|
|9|Pcm|12|9,342|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|10|Atom|13|147,067|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|11|Flight|13|150,000|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|12|Tax|15|12,106|[FastDD-Exp](https://github.com/TristonK/FastDD-Exp/blob/8e284e925a671749f1ae73017c6adf8013397316/datasets.zip)|
|13|Adult|15|32,561|[UCI](https://archive.ics.uci.edu/dataset/2/adult)|
|14|Depression|16|413,768|[Kaggle](https://www.kaggle.com/code/pritesbera/depression-data-eda?scriptVersionId=198947839)|
|15|Evehicle|17|181,458|[OpenML](https://www.openml.org/search?type=data&status=active&id=45948)|
|16|Sgemm|18|241,660|[UCI](https://archive.ics.uci.edu/dataset/440/sgemm+gpu+kernel+performance)|
|17|Software|21|89,324|[HPI](https://hpi.de/naumann/projects/repeatability/data-profiling/fds.html)|
|18|Structsite|27|134,076|[HPI](https://hpi.de/naumann/projects/repeatability/data-profiling/fds.html)|
|19|Reflns|37|24,769|[HPI](https://hpi.de/oldsite/fileadmin/user_upload/fachgebiete/naumann/projekte/repeatability/Pyro/REFLNS.csv.bz2)|
|20|Sonar|60|208|[OpenML](https://www.openml.org/d/40)|
|21|Movement|91|360|[NetworkRepository](https://networkrepository.com/movement-libras.php)|
