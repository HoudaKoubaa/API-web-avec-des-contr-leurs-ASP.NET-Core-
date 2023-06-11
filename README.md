# API web avec des contrôleurs ASP.NET Core 
 Crud Pizza Avec  ASP.NET core 
# Générer et exécuter l’API web 

1. dotnet run 
Rouvrez le terminal httprepl existant ou un nouveau terminal intégré depuis Visual Studio Code en sélectionnant Terminal>Nouveau terminal dans le menu principal.
2. httprepl https://localhost:{PORT}
3. connect https://localhost:{PORT}

4. Accédez au point de terminaison Pizza en exécutant la commande suivante :
    cd pizza 
5. Exécutez la commande suivante pour voir les nouvelles actions sur l’API Pizza :
    ls

Sortie => 

    https://localhost:{PORT}/Pizza> ls
    .      [GET|POST]
    ..     []
    {id}   [GET|PUT|DELETE]

6. Effectuez une requête POST pour ajouter une nouvelle pizza dans HttpRepl en utilisant la commande suivante :
   post -c "{"name":"Hawaii", "isGlutenFree":false}"

7. Mettez à jour la nouvelle pizza Hawaii en pizza Hawaiian avec une requête PUT en utilisant la commande suivante :

put 3 -c  "{"id": 3, "name":"Hawaiian", "isGlutenFree":false}"

8. Notre API peut également supprimer la pizza nouvellement créée avec l’action DELETE en exécutant la commande suivante :
    delete 3
