# experience_mulesoft_exo
 
## Application 3
Créer des specs api permettant de récupérer les données via un endpoint /contracts en utilisant la methode “GET”
Créer un flow “fetch-data” qui va récupérer les données depuis “Application2” et retourner un payload de pair / impair en fonction de la valeur du payload.
Créer un flow “reformat-data” qui va definir un payload au format texte dans un TransformMessage de la forme suivante:

Voici la liste des contrats:
Contrat avec l’id paire :
(lookup vers le flow “fetch-data” pour récupérer les contrats pair)
--------------------
    "Contract_ID": "10",
    "Creation_Date": "21-02-2019",
    "Start_Date": "30-04-2018",
    "End_Date": "30-04-2019",
    "Customer_ID": "301207461",
    "Salesman_ID": "800023000126",
    "SalesUnit_ID": "21M233COPL-EVFR-01",
    "Amount": "23250.000000",
    "Contract_Name": "",
    "Currency_Code": "EUR",
    "Renew": "",
    "Customer_Name": "",
    "Salesman_Name": "",
    "SalesUnit_Name": "",
    "Number_Of_Months": 12.03,
    "Opportunity_ID": null,
    "CUTOFF_MONTH": "01-04-2018",
    "CUTOFF_AMOUNT": 64.4,
    "amount_per_month" : 100
--------------------
...

Contrat avec l’id impaire :
(lookup vers le flow “fetch-data” pour récupérer les contrats impair)




Appeler le flow “fetch-data” depuis le flow généré par les spec api
(S’il y a le temps) Ajouter le protocol https en suivant ce tuto : tuto https

