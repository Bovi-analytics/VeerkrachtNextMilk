# Repository for nextMilk prediction of Veerkracht

## The dataset

In the './Data/' folder a dataset of individual cow milk recording events of 100 farms has been collected.

The dataset is partitioned into 10 partitioned csvs (UTF-8 charset) each containing milk recordings

* Default timestamp format is yyyy-MM-dd'T'HH:mm:ss[.SSS][XXX]
* Default line seperator is  \n

Eah row of the dataset contains:

* HerdIdentifier - Unique identification number of the farm - string
* AnimalIdentifier - Unique identification number of the animal - string
* BirthDate - Birth date of the animal - timestamp
* CalvingDate - Calving date of the lactation - timestamp
* LactationNumber - Lactation number of the lactation - integer
* TestDate - Date of milk recording - timestamp
* MilkYieldKg - Milk yield of the milk recording - double
* DaysInMilk - Days in milk at the milk recording - integer
* FatPercentage - Fat content (%) of the milk recording - double
* ProteinPercentage - Protein content (%) of the milk recording - double

## Goal of each partner

Please create a folder in the './Predictions/' with your own milk yield predictions using the same unique identifiers