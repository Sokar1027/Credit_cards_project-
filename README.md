# Credit cards clustering analysis

## Unsupervised learning analysis of 234 credit card products in Colombia to identify customer segments. Using K-Means and Agglomerative Clustering, 3 distinct clusters were identified representing high-capacity, special, and standard customer profiles. These insights can inform product development and market segmentation strategies

### The goal of this project was to identify and understand the main customer segments based on credit card characteristics, and to explore whether the model could reveal additional groups that provide deeper insights into customer behavior

## Dataset
### Data source: https://www.comparaonline.com.co/tarjeta-de-credito
### 234 records, 12 features (after the wrangling proccess)
### Features:
  - nombre_tarjeta (Name of the credit card)
  - Tasa de interés mensual (Monthly interest rate applied to the card)
  - Ingreso mínimo (Minimum income required to apply for the card)
  - Cuota de manejo (Monthly maintenance or management fee for the card)
  - Marca (Brand or network of the card (e.g., Visa, Mastercard))
  - Solicitar (Link or option to apply for the card)
  - Costo de avance en efectivo (Cost or fee charged for cash advances)
  - Tipo de tarjeta (Indicates whether the card is national or international)
  - Tasa de interes no informada (Boolean variable indicating whether the interest rate information is missing (1 = not informed, 0 = informed))
  - Ingreso minimo no informado (Boolean variable indicating whether the minimum income information is missing (1 = not informed, 0 = informed))
  - Disponibilidad (Boolean variable indicating whether the card is available (1 = available, 0 = not available))
  - Banco (Bank that issues the card)


## Metodology
### Scraping:
  - Web scraping from ComparaOnline web site
### Wrangling:
  - Treatment to each column
  - Input data to replace the missing values
  - creation of two new flags for helping the training model
### EDA:
  - Distribution visualization and correlation inspection
  - Search of patterns and insights into the data
### ML: 
  - Models used: K-means and Agglomerative clustering
  - Evaluation methods: Sillhouette score and Elbow method
  - Interpretation and insights oriented analysis of each cluster

## Principal insights and conclusions
  - after the analysis the model could identify the three usual groups that the costumers usually are divided; standard client, high economic capacity client, special client.
  - Most of the feature overlap with each others, it's difficult to see a clear separation in them. About it, we can infer that these features aren't important to the model.
  - Unlike the others features, interest rate feature seems important to the model, as there is a clear separation between the clusters.

## Technologies:
 - Selenium
 - Pandas
 - Numpy
 - Matplotlib
 - Seaborn
 - Scikit-learn
 - Python
 - Jupyter notebooks

# Note: Some comments and titles were reviewed and improved with the assistance of ChatGPT for clarity and English refinement. All insights, model selection, analysis, and project decisions are my own.
