# 📊 SheetDB 📊
Convertint fulls de càlcul en una base de dades en línia  

## ℹ️ Què és SheetDB?

**SheetDB** és una tecnologia que permet convertir un **full de càlcul de Google Sheets** en una **API REST**, fent possible accedir, consultar, afegir, modificar o eliminar dades mitjançant peticions HTTP.  
Aquesta eina actua com un pont entre els fulls de càlcul i les aplicacions web, permetent treballar amb dades de manera estructurada sense necessitat de crear una base de dades tradicional.  

## 📝 Què aprendrem a fer amb SheetDB?
- Entendre com un **full de càlcul pot funcionar com una base de dades**.  
- Crear una **API REST** a partir d’un Google Sheet.  
- Fer consultes de dades mitjançant **peticions HTTP**.  
- Afegir, modificar i eliminar registres de forma remota.  
- Relacionar dades de diferents fulls com si fossin **taules d’una base de dades relacional**.

👉 **Exemple:**  
[https://sheetdb.io](https://xbaubes.github.io/modules/aplicainfo/fullAPI/fullAPI.html?page=Full%20de%20c%C3%A0lcul%20com%20a%20API)

---

## 🔌 Pràctica: Fulls de càlcul com a API

Pots utilitzar les dades que vulguis

**1. Dissenyar i omplir Google Sheets**

- Defineix pestanyes i columnes.
Crea almenys dues pestanyes amb informació relacionada entre elles.

| Pestanya 1 : Sagues     | Pestanya 2 : Enemics     |
|-------------------------|--------------------------|
| ![Sagues](Sagues.png)   | ![Enemics](Enemics.png)  |

- Insereix dades reals: Omple cada pestanya amb dades entrellaçades.

- Defineix una relació entre les taules: Utilitza una clau forana.

Exemple relació 1:N -> Una saga té molt enemics i un enemic pertany a una sola saga
![Diagrama](diagrama.jpg)

- Crea un diagrama que representi la relació que has creat.

**2. Crear compte SheetDB**

- Crear una API pel full de càlcul generat, assegura't que és d'accés públic.

- Obté la URL base de l'API: Aquesta URL permetrà consultar i modificar les dades.

**3. Defineix les crides a l'API**

Fes captures de pantalla de la resposta rebuda.

- GET (consulta de dades)

Obre el navegador amb la URL base per veure dades d'una pestanya. Canvia la ordenació per defecte dels resultats.

![Resultat GET](GET.png)

(terminal CMD - cURL)
- Inserció de dades (POST)
- Modificació de dades (PUT)
- Eliminació de dades (DELETE)

Comanda cURL POST genèrica:
curl -X POST https://sheetdb.io/api/v1/<API_ID>?sheet=<NOM_PESTANYA> -H "Content-Type: application/json" --data-binary @<RUTA_FITXER_JSON>

https://sheetdb.io/api/v1/<API_ID>?sheet=<NOM_PESTANYA>

<API_ID> → Identificador únic de la teva API generada per SheetDB.

?sheet=<NOM_PESTANYA> → Nom de la pestanya del full de càlcul on vols inserir les dades (ex: “Enemics”).

-H "Content-Type: application/json"

Capçalera que indica que les dades enviades són en format JSON.

--data-binary @<RUTA_FITXER_JSON>

@<RUTA_FITXER_JSON> → Ruta al fitxer JSON que conté les dades a afegir.

El fitxer JSON ha d'estar ben formatat. [Descarregar post_enemic.json](post_enemic.json)

Guardar la petició HTTP POST en un fitxer JSON i indicar amb quina comanda s'utilitza.

**4.** [OPCIONAL] **Implementació web**
- Crea una petita aplicació web (HTML + JS) que consumeixi l'API creada.
