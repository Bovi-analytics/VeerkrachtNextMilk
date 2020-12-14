# Repository for nextMilk prediction of Veerkracht

## About

This repository contains data to validate the next milk predictions from the Veerkracht VLAIO project. Please request write access to the repository via m.m.hostens@uu.nl
If extra information is needed, this can be requested.

## The dataset

In the './Data/' folder a dataset of individual cow milk recording events of 100 farms has been collected.

The dataset is partitioned into 10 partitioned csvs (UTF-8 charset) each containing milk recordings

* Timestamp format is 'yyyy-MM-dd'T'HH:mm:ss[.SSS][XXX]'
* Line seperator is  '\n'
* Seperator is ','

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

The predictions for the first milk yield prediction should have the following format

* HerdIdentifier - Unique identification number of the farm - string
* AnimalIdentifier - Unique identification number of the animal - string
* CalvingDate - Calving date of the lactation for which the first yield is pedicted - timestamp
* LactationNumber - Lactation number of the lactation - integer
* TestDate - Date of milk recording - timestamp
* MilkYieldKg - Milk yield (kg) of the milk recording - double
* DaysInMilk - Days in milk at the milk recording - integer
* PredictedMilkYieldKg - Predicted milk yield (kg) - double