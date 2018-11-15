# StreamIT.TO Api #
#### Api Key erstellen ####
**Endpoint**: /api/NewKey

**Method**: GET
- $key
- $length (optional)

Example:
```php
http://localhost/api/NewKey?key=$key&length=$length
```

#### Media Stream hinzufügen ####
**Endpoint**: /api/AddStream

**Method**: GET
- $key
- $IMDB (optional)
- $MediaStream
- $MediaType (movie/tvshow)
- $MediaIMG
- $MediaSound
- $MediaLang (de/en)
- $Staffel (nur Serien)
- $Episode (nur Serien)
- $EpisodeName (nur Serien)


Example:
```php
http://localhost/api/AddStream?key=$key&IMDB=$IMDB&MediaStream=$MediaStream&MediaType=$MediaType&MediaIMG=$MediaIMG&MediaSound=$MediaSound&MediaLang=$MediaLang
```

#### Media hinzufügen ####
**Endpoint**: /api/AddMedia

**Method**: GET
- $key
- $IMDB
- $MediaType (movie/tvshow)
- $MediaLang (de/en)

Example:
```php
http://localhost/api/AddMedia?key=$key&IMDB=$IMDB&MediaType=$MediaType&MediaLang=$MediaLang
```



#### Error Codes
Api Error Codes:
-   1: Falscher Api Key
-	2: Kein Api Key gesetzt
-	3: Keine methode für die api gesetzt
-	4: Api Parameter prüfen
-	5: Episoden oder Staffel Parameter fehlt
