# Crime Factors

Crime is a huge political subject in France. Its causes are also subject of intense political debate.
Different factors going from immigration to poverty have been proposed, but evidence seems to be lacking in the political debate. 


This project tries to show the impact of different factors at the departemental level using linear models. An interactive map will be made allowing the user to select the factors and see their impact on crime.

## Data sources

### Crime

The main dataset is the [crime dataset](https://www.data.gouv.fr/fr/datasets/chiffres-departementaux-mensuels-relatifs-aux-crimes-et-delits-enregistres-par-les-services-de-police-et-de-gendarmerie-depuis-janvier-1996/) it contains number of mensual crimes reported to the police per departement for 106 categories of crime(examples include "Règlements de compte entre malfaireurs", "Infractions à la législation sur les chèques", and "Autres délits économiques et financiers"). For simplification purposes two strategies are considered either grouping the 106 categories into fewer more general categories or just adding all different categories of crime into one crime indicator. 



This dataset includes data on crime back to 1996 for most departments however, for overseas France some years are missing. This website will focus on mainland France as overseas France has unique circumstances which will biais te data. Linear models will use crime data from 2017 as most of the other indicators come from the years 2016-2à17. Data is mensual but has been grouped by year by us for easier analysis. 


The data is in the form of an excel spreadsheet with one sheet per departement, this form of data is being transformed to a more usable csv format.


![Alt text](relative/path/to/img.jpg?raw=true "Title")


### Population

The crime dataset and other datasets are not adjusted for population as such a [population dataset](https://www.insee.fr/fr/statistiques/2012713) is needed. This dataset does not contain the population for every year but does have the year 2017 which will be the one used in this project. Data is at a departmental level.


### Schooling


As an bad approximation for school success in an departement we will be using the [percentage of success at the BAC](https://www.insee.fr/fr/statistiques/2012792) a french national exam. Data is from 2019 and is per departement.


### Unemployement


[Unemployement percentage](https://www.insee.fr/fr/statistiques/2134411) is available at a departemental level for the year 2019.


### Immigration

[Immigration data](https://www.insee.fr/fr/statistiques/2012727) is available for the year 2017. It contains the percentage of immigrants in each departement, plus the percentage of each nationality if further analysis is desired.


###  Poverty

[Poverty rate](https://www.insee.fr/fr/statistiques/2012803) is here. The data is by age.


 


Maps come from [france geojson](https://github.com/gregoiredavid/france-geojson)


## Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app). In order to run this project you need [node.js](https://nodejs.org/en/)

In the project directory, you can run:
### `npm install`

Installs the required dependencies **including** d3. 

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.



### `npm build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.



### Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
