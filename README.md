<a id='francais'></a>
<h1>chaines de caractère</h1>
<a href='#english'>in English</a>
<h2>En un mot</h2>
L'objectif de l'outil est de repérer des datasets Recherche Data Gouv qui devraient être transvasés d'un dataverse à un autre
<br/><br/>
Pour cela il va chercher une ou plusieurs chaînes de caractères entrées par l'utilisateurs dans les zones "publisher" et "producers" des datasets
<h2>Utilisation</h2>
L’utilisateur se voit présenter une zone d'input dans laquelle il peut mettre une ou plusieurs chaines de caractères, ainsi qu'un choix de dates
<br/><br/>
Il recoit une liste de datasets classés par dataverse. Pour chaque dataset : le nom, avec un lien, la descrition, le publisher, les producers
<h2>Langage</h2>
HTML, JavaScript
<br/><br/>
N'importe quel browser permet d'utiliser le code
<h2>Fichiers</h2>
Pour permettre une instalation la plus facile possible tout le code (toutes les fonctions) se trouve dans un seul fichier, xxx.html
<h2>Dépendance</h2>
L'outil est dépendant des API de Recheche Data Gouv telle qu'elles existent aujourd'hui (mars 2025) avec le point d'entrée https://entrepot.recherche.data.gouv.fr/api/search
<h2>Fonctionnement, fonctions</h2>
La fonction send_function() lance le processus, elle est déclenchée par le bouton du formulaire
<br/><br/>
La fonctin get_data_function() va chercher les données, via un fetch
<br/><br/>
La fonction can_data_function() stocke les données, dans trois variables : dataset_data_object, dataverse_data_object, data_structure_object
<br/><br/>
La fonctin display_data_function() affiche les données
