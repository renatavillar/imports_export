# imports_export
A study of Brazil's exports and imports of some products. I used the following data: <a href=http://comexstat.mdic.gov.br/>Comexstat</a> and <a href=https://github.com/renatavillar/imports_export/blob/master/covariates.xlsx/>Covariates</a>. It was a challenge proposed in a selection process. I worked in two cases:

### Case 1
I used the dataset 'TFP.csv'. I worked mainly on two topics for this case:
- A an exploratory data analysis;
- A 10-years forecast extrapolating the series;

### Case 2
I used data from <a href=http://comexstat.mdic.gov.br/>Comexstat</a> and <a href=https://github.com/renatavillar/imports_export/blob/master/covariates.xlsx/>Covariates</a>. The dataset contains all trackings of monthly imports and exports of a range of products (soybeans, soybean meal, soybean oil, corn, wheat and sugar), by brazilian states, by routes (air, sea, ground, etc) e from/to which country;
I worked mainly on the following topics:
- Show the evolution of total monthly and total annual exports from Brazil (all states and to everywhere) of ‘soybeans’, ‘soybean oil’ and ‘soybean meal’;
- To find the 3 most important products exported by Brazil in the last 5 years;
- To find what are the main routes through which Brazil have been exporting ‘corn’ in the last few years and if there are differences in the relative importance of routes depending on the product;
- Which countries have been the most important trade partners for Brazil in terms of ‘corn’ and ‘sugar’ in the last 3 years;
- For each of the products in the dataset, to find the 5 most important states in terms of exports;
- To build a model in order to predict the total annual exports of brazilian soybeans, soybean_meal and corn, in tons, for the next 11 years (2020-2030).

I am working on the model, to get a good fit (it is far away of being well fitted). By now, I think XGBoost is the best option, but any suggestion to get a good fit is welcome. The correlation of the response variable with each of the features is extremely bad, as we can see in notebook case2.ipynb. We need to colect more features, outside the given dataset. We need features that explain the target variable (tons).
