Ce projet SKF récupère des paramètres et les compare à un fichier XML présent dans le projet.

Le résultat des tests dépendent donc de ce qui est envoyé.

Ce projet est composé de 5 cas de test, chacune avec un type de paramètre attendu :

ecosystem/compareXmlTSCUF.ta : Test présent dans un écosystème. Le setup.ta et teardown.ta sont juste des inscriptions
dans les logs. Vérifie l'envoi de CUF au niveau des suites de test.

ecosystem2/compareXmlCPGCUF.ta : Test présent dans un écosystème. Le setup.ta et teardown.ta sont juste des
inscriptions dans les logs. Vérifie l'envoi de CUF au niveau de la campagne.

compareXmlDataset.ta : Test à la racine du dossier "tests". Vérifie l'envoi de jeux de données.

compareXmlITCUF.ta : Test à la racine du dossier "tests". Vérifie l'envoi de CUF au niveau de l'itération.

compareXmlTCCUF.ta : Test à la racine du dossier "tests". Vérifie l'envoi de CUF au niveau du cas de test.

Pour que le test se termine en succès, il faut récupérer et envoyer un label existant présent dans resources/xml-resources/initial.xml

Exemple de valeurs acceptées :

CPG_CUF_clockspeed : 3.6 / 3.9

DS_label : Intel i9-9900K / AMD Ryzen 9 3900X

IT_CPG_socket : LGA 1151 / AM4

TC_CUF_price : 600 / 445

TS_CUF_threads : 8 / 16 / 24

Le fichier customsuite.json est disponible à la racine du projet pour une exécution en ligne de commande.