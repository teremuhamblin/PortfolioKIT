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

### PortfolioKIT propulsé par Next.js et Nextra.

​1. *Déploiement rapide sur Vercel* (Recommandé)
```text
- ​Vercel est l'hébergeur idéal créé par les concepteurs de *Next.js*.
- *Le déploiement y est entièrement automatisé*.
- **​Créez un compte sur Vercel** si ce n'est pas déjà fait.
- ​Cliquez sur **Add New... > Project**.
- *​Importez votre dépôt GitHub PortfolioKIT*.
```

》》 ​Vercel détectera automatiquement qu'il s'agit d'un projet *Next.js*.
​Cliquez sur Deploy.

》》 ​À chaque fois que vous ferez un git push sur la branche main.

>> **Vercel déploiera automatiquement votre mise à jour**.

### Configuration post-déploiement

​Avant de finaliser votre mise en ligne, assurez-vous d'avoir configuré :

- ​L'URL du site : *Mettez à jour l'URL de production dans* **scripts/gen-rss.js** *pour que le flux RSS pointe vers votre domaine final*.

- ​Les variables d'environnement : *Si votre site nécessite des clés d'API (pour un formulaire de contact par exemple), configurez-les dans les paramètres du projet sur Vercel*.

### Déploiement alternatif (GitHub Pages ou VPS)

​Si vous préférez héberger votre site ailleurs qu'sur Vercel :

- ​**Export statique** : *Vous pouvez configurer Next.js en mode export statique (output: 'export' dans next.config.js) pour générer un dossier de fichiers HTML/CSS/JS purs*.

- ​**Hébergement** : *Ces fichiers statiques peuvent ensuite être hébergés sur* **GitHub Pages, Netlify, ou un serveur web classique (Nginx / Apache**)

```text
​with open('docs/guide.md', 'w', encoding='utf-8') as f:
f.write(guide_content)

​with open('docs/deployment.md', 'w', encoding='utf-8') as f:
f.write(deployment_content)
​print("Files generated successfully.")
```
