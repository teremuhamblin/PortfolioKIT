###### GUIDE.md >> markdown 

# PortfolioKIT

## Guide d'utilisation 

### Syntaxe Markdown de base

- ​Le Markdown vous permet d'écrire du texte enrichi sans complexité :
​Titres :

```text
- Utilisez " # " pour un titre principal (<h1>).

- Utiliser " ## " pour un sous-titre (<h2>), etc.

- ​Gras et Italique : **texte en gras** et *texte en italique*.

- ​Listes : Utilisez des tirets - ou des astérisques * pour les listes à puces.

- ​Liens : [Intitulé du lien](https://exemple.com)

- ​Images : ![Description de l'image](/images/mon-image.png)
```

​### Utilisation de MDX

- 》》 **Composants React**
​Le grand avantage de Nextra est le support de MDX, qui vous permet d'intégrer directement des composants React ou des éléments interactifs au milieu de votre texte Markdown.

》》 **import { Callout } from 'nextra-theme-docs'**

### Mon article avec des composants

Voici un paragraphe standard.
```markdown
<Callout type="info" emoji="💡">
  Ceci est une boîte d'information interactive intégrée directement dans votre article Markdown !
</Callout>
```

```markdown
<Callout type="warning" emoji="⚠️">
  Attention à bien importer vos composants si nécessaire.
</Callout>
```

### Intégration de blocs de code

​Pour insérer du code source avec coloration syntaxique :

```javascript
// Exemple de code JavaScript
function saluer(nom) {
  console.log(`Bonjour, ${nom} !`);
}
saluer("Développeur");

"""
​
deployment_content = """# Guide de déploiement en production
```

>> ​Ce guide détaille les étapes pour mettre en ligne votre portfolio
