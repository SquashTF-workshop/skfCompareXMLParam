Ce projet SKF récupère les paramètres envoyés depuis Squash TM et les compare à un fichier XML présent dans le projet.

Le résultat des tests dépendent donc de ce qui est envoyé.

Un test utilise les jeux de données, tandis que l'autre utilise les CUF du cas de test.

Ces deux paramètres doivent s'appeler "label".

Pour que le test se termine en succès, il faut récupérer et envoyer un label existant présent dans resources/xml-resources/initial.xml

Exemple de valeurs acceptés : 

Intel i9-9900K
AMD Ryzen 9 3900X
Intel i7-9700K