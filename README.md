# Bot-Resume-Sender
Bot who send my Resume for me 

--- 
J'en ai marre d'envoyer des CV pour ma recherche de stage, c'est fatiguant et c'est répétitif ! Ce repesitory est un rappel à moi-même de créer un bot qui envoie un nombre N de CV selon certains critère de recherche et certain mots clés présent dans l'offre (linkedIn ou toute plateforme qui demande juste d'envoyer son CV).

Pour ce faire :

> Etape 1 : Récupérer de la données
- BDD de poste IA qui m'interresse 
- Créer un fonction qui recupere une ligne de future data d'offres, à partir d'un lien `ma_fonction(search_url)`. Récuperer une dizaine de lien et executer le bail dessus. Faire du nlp, analyse pour voir les similitudes, récurrences, les mots clé que je dois absolument ajouté à mon CV. Le but est aussi de comprendre ce que je recherche réellement et le point commun de mes recherches, ce qui fait que ça me plait. Ajouter les infos de l'entreprise.
- Creer un code capable d'ajouter des mots clés en soum, dans un pdf. Le but sera d'ajouter des mots clé à mon CV automatiquement en insérant la description de l'offres de stage dans le programme.
- Creer un fonction qui récupère TOUTES les offres à partir d'un mot clé de recherche et des mots clé obligatoire `ma_fonction(search_title, mandatory_keyword = ["IA", "Python"], count=50) `

*Objectif final* : Creer un algo qui, après execution, me ressort un excel avec les offres de stage du jour à postuler

> Etape 2 : 
- Prendre des offres que je veux pas. Faire attention à la proportion du type d'offre que je veux VS. le type d'offre que je veux pas.
- Entrainer plusieurs modèles et les comparer.

*Objectif final* : Creer un algo capable de prédire si ce truc peut m'interresser ou non.

> Etape 3 : 



*Objectif final* : Creer un algo envoie mon CV à ma place aux offres qui pourrait m'interresser.

---

```python
data = None
for mot_cle in ["IA/AI", "NLP", "MachineLearning", "AlgorithmeGenetique/GeneticAlgorithme", "Python", "Data"]:
   data.append(save_offers_to_excel(mot_cle, count=50))

data = pd.concat(data)

do_nlp(data)

````

Note : à finir avant 2023
