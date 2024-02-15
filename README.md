## DESCRIPTION

** WORK IN PROGRESS

### Branch B - Health-Nutrition and Population Statistics (HNP Statistics)


## WORKFLOW

1. Data downloaded locally from the World Bank IBRD-IDA (Link below) 
2. Data was inspected and transformed using Python. The entire dataset was narrowed to focus on information related to population behaviour, which is the topic of the interest, for now.

The main take aways from this step are:

- Data extracted is related to population dynamics & structure, life expentancy and mortality & death indexes. At world, region and country scale.
- Data was divided into five dataframes, where each one contains one topic of the ones aforementioned. Dataset was designed aiming to work as relational database.
- Raw data came in a wide format. It was decided to reshaped the data in a long format, eventhough memory usage was increased slightly. Now, the data is in a more friendly user format and ready for further analysis.
          
3. Dataset imported to Tableau for developing an interactive dashboard about World population.

Files:

- Jupyter notebook: Python code saved as jupyter and html format. File name: 'data_transformation.html' and 'data_transformation.ipynb'
- Data source link: [Data Source](https://datacatalog.worldbank.org/search/dataset/0037652/Health-Nutrition-and-Population-Statistics)
- Tableau link: [Interactive dashboard: World Population](https://public.tableau.com/views/HNPstats/Populationoverview?:language=en-US&:display_count=n&:origin=viz_share_link)

### [Go Back](https://github.com/luis12pez/Tableau-viz)
