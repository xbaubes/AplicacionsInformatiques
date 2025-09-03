# Google Workspace

## ℹ️ Què és Google Workspace?

**Google Workspace** és un conjunt d’eines en línia de Google (Gmail, Drive, Docs, Sheets, Slides, Forms, Sites, Calendar, etc.) pensades per treballar, comunicar-se i col·laborar de manera integrada.

---

## 📝 Presentació de la pràctica

En aquesta pràctica aprendrem a utilitzar diverses eines web de Google de manera col·laborativa.  
El treball es farà en **grups de 2 o 3 persones**, aprofitant les opcions de col·laboració en temps real.  

La tasca principal consisteix a **crear una enquesta de tema lliure**, difondre-la per obtenir respostes i, finalment, **publicar els resultats en una pàgina web**.

👉 Exemple orientatiu:  
[Pàgina web amb enquesta i resultats analitzats](https://sites.google.com/xtec.cat/enquesta-programacio)

## 📌 Planificació

La pràctica s’ha de fer seguint aquest ordre de passos i fites:

### Pas 1
- Definir tasques i assignar responsables a **Trello**.  
- Crear l’enquesta inicial amb **Google Forms**. Cal que l'enquesta estigui preparada a temps per a fer-ne la difusió i la recollida de respostes.  

### Pas 2
- Pàgina web de **Google Sites** estructurada i publicada.  
- Generar un **Google Sheets** a partir de l'enquesta on s'hi volcaran les respostes automàticament. Cal processar les dades i generar gràfics que s'inclouran a la pàgina web.  

### Pas 3
- Preparació de l’informe amb **Google Docs** i presentació final del projecte.  

⚠️ Els grups que no respectin aquesta planificació podran ser penalitzats.

## 🔧 Desenvolupament

Les eines de Google que utilitzarem són:

- **Google Forms** → per elaborar el formulari de l’enquesta i recollir respostes.  
- **Google Sheets** → per analitzar les dades i generar gràfics.  
- **Google Docs** → per redactar l’informe amb resultats i conclusions.
- **Google Sites** → per crear el lloc web i publicar l’enquesta i els resultats.  

### Preparació inicial
1. Creeu una carpeta al **Google Drive** anomenada:  
   `GoogleWorkspace-enquesta-membre1-membre2-membre3`  
   (substituint *membreN* pel nom i cognom de cada integrant).  
2. Compartiu la carpeta amb **permís d’edició** amb els companys del grup.  
3. Configureu la carpeta com a **només lectura** per a qualsevol persona amb enllaç.  
4. Dins la carpeta, guardeu tots els arxius que utilitzeu per completar la pràctica (Forms, Sheets, Docs, Sites, pdf i imatges si ho creus necessari).  

💡 Recomanació: que cada membre investigui una eina diferent i aporti coneixements al grup. Es pot començar amb una **enquesta de prova** abans de fer la definitiva.

## 📋 Google Forms

El formulari ha de complir amb aquests requisits mínims:

- Entre **5 i 10 preguntes**.  
- Com a mínim una de tipus **Multiple choice** i una altra **Checkboxes**. Almenys una d’elles amb opció “Altres” per escriure respostes.  
- Almenys **una pregunta obligatòria**.  
- Una pregunta amb **imatges a les respostes** i una altra amb **imatge il·lustrativa** de la pregunta.  
- Organització en **seccions** amb **barra de progrés**.  
- **Tema visual coherent** amb el disseny del web.  
- Limitar a **una resposta per compte**. Valora si és adequat que es permeti editar les respostes un cop enviat
- Per complir amb la normativa de protecció de dades, no es permet la recollida de les adreces electròniques.

👉 Exemple:
[Trivial Pursuit](https://forms.gle/XwYoTPDCskCrNrBE6)

## 📊 Google Sheets

- **Emmagatzemar** totes les respostes de l’enquesta automàticament. Enllaçarem un full de càlcul per guardar les respostes des de la pestanya «Respostes» de la vista d’edició.
- **Netejar** les dades introduïdes des de teclat per l’usuari i processar-les correctament. Per exemple, eliminant espais sobrants (=TRIM(...)) i separant en diferents respostes els textos que incloguin comes (=SPLIT(...)).
- **Anàlisi de les dades** i elaboració de gràfics per a l'informe de resultats.
- **Crear diferents tipus de gràfics**, utilitzant el tipus més adequat per a cada pregunta.
- **Almenys un dels gràfics ha de mostrar la relació entre les respostes de dues preguntes diferents del formulari.** Per exemple, després de preguntar l’edat i l’interès en varis temes, cercar la relació entre l’interès per un tema determinat i l'edat.
- Afegir un **contador automàtic de respostes** (=COUNTA(...)).
- Assegura’t que automàticament s’agafen totes les files per generar els gràfics.

## 📑 Google Docs

L’informe haurà de contenir:

- **Portada** amb títol i autors.  
- **Taula de continguts**.  
- **Capçalera**.  
- S'ha d'afegir **gràfics** de resultats des del full de càlcul de respostes i des dels gràfics que genera automàticament Google Forms.
- S’han d’analitzar detalladament els resultats obtinguts fins aquell moment i anotar-ne la data en l’informe.
- Conclusions i possibles millores.  
- S'haurà d'exportar en format PDF per tal que pugui ser descarregat mitjançant un enllaç a la web.

## 🌐 Google Sites

El lloc web haurà d’incloure:

- Dissenyar l'aspecte del lloc web:
  - Disseny personalitzat amb **logo, banner i favicon**.
  - Escollir i personalitzar un tema.
- Un mínim de **3 pàgines**:
  - Benvinguda: Explicació del projecte.
  - Enquesta: Explicació de la temàtica del formulari i enllaç per accedir-hi.
  - Resultats: Gràfics que organitzen les respostes rebudes, contador automàtic amb el nombre de respostes i enllaç per descarregar l'indorme en pdf.
      - Inserció de gràfics enllaçats (no imatges estàtiques). Inclou tant gràfics generats pel Google Forms com del full de càlcul. S'han d'inserir com a gràfics o amb <iframe> per tal que estiguin enllaçats i s’actualitzin amb cada nova resposta. 
