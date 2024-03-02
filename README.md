# f3-AnnotationRouting

Configurationn des routes de fat-free-framework avec des Dockblocks

## Exemple 1 route normale :
```
class MaClasse {
  /**
  * @route("GET /")
  **/
  function MaMethode (...) {
  // Code de la méthode
  }
}
```

 **est équivalent à** 
```
$f3->route('GET /', 'MaClase->MaMethode');
```
## Exemple 2 route avec ajax :
```
class MaClasse {
  /**
  * @ajax
  * @route("GET /list")
  **/
  function MaMethode (...) {
  // Code de la méthode
  }
}
```

 **est équivalent à** 
```
$f3->route('GET /list  [ajax]', 'MaClase->MaMethode');
```
