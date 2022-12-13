# ApiAlbum
creer un projet android studio 
1) Soit l'API get https://jsonplaceholder.typicode.com/albums/1/photos, tester l'API sur votre navigateur et créer la classe Photo correspondant aux données JSON affichées (1pt)
2) on veut consommer l'API en utilisant retrofit (5pt)
    a)ajouter les dépendances nécessaires au projet
    b) préparer l´interface api Photos néssaire contenant la méthode getPhotos   
    c)préparer l´objet RetrofitHelper permettant d´instancier la bibliothéque retrofit  
    d)consommer l'api et afficher le résultat sur le console.  
 
 3) on veut afficher la liste de photos comme suit:(5pt)<br/> 
    <img src="https://github.com/mouniraz/ApiAlbum/blob/main/ds.JPG" />
    <br/>
     a) préparer un composable ItemPhoto(photo:Photo) qui affiche le titre et l´image    
     b) préparer un composable ListPhoto(photos:List<Photo>) permettant d´afficher une liste de ItemPhotos  
     c) afficher la liste de photos, le résultat du méthode get ce-dessus    
    
  Execution correcte sur 4pt
    
  4) Réellement, les photos dépendent de l'id de l'album 
    https://jsonplaceholder.typicode.com/albums/{id}/photos
    si on change l'id, le résultat change, pour celà on veut améliorer l´interface comme suit:<br/>
    <img src="https://github.com/mouniraz/ApiAlbum/blob/main/Captureds2.JPG" height="200"/><br/>
    a) implementer la fonction composable Form qui contient la zone de saisie AlbumId et le button search comme suit 
    <img src="https://github.com/mouniraz/ApiAlbum/blob/main/Captureds3.JPG" />
    b) afficher l´interface finale contenant la Form et la liste de photos  
    c) ajouter la méthode    
       ``kotlin
    @GET("albums/{id}/photos")

        ....getPhotobyAlbum(@Path("id") id:Int).....
    ``
