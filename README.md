# api_miner
series of functions to mine the Materials Project Battery Explorer as well as the materials database
the primary output are a csv file of the features and a csv files of the labels used in our paper:

note that to use these scripts, you must have an account on Materials Project (free) so you can generate your own MAPI key
(if you find my MAPI key on my scripts, please let me know)
(see scripts API Miner)

## Battery API Miner Folder
one script which queries the Battery Explorer and mines them to a text file in a directory that is currently named Battery_Explorer

## Materials API Miner Folder
two core scripts - one which mines materials data and structure data to json format in one file each (Materials_Project_Database)
                 - second one mines the structure into a pymatgen structure object, stored as a pickle file (structure_base)

## mining the api extracted data
there is an additional set of functions which further mines the raw database to generate features and labels
for battery machine learning, which is a separate repository you can check to see state of the art machine learning algorithms

## data-dump
we include a folder called data-dump where I usually put in all the .csv files which are successfully mined from the data-miner
these files should be transferred to the battery machine learning repo for further analysis. we want to keep things as compartmentalized as possible
