# PortfolioKIT

Ce portfolio est construit avec *Next.js* et *une bibliothèque appelée Nextra*.
- Elle vous permet d’écrire en *Markdown* et de vous concentrer sur le contenu de votre portfolio.

### Ce starter inclut 
```text
- Configuration automatique pour gérer Markdown/MDX  
- Génère un flux RSS basé sur vos articles  
- Un thème magnifique inclus par défaut  
- Catégorisation facile des articles avec des tags  
- Chargement rapide et optimisé des polices web  
```

### Configuration
```text
1. Mettez à jour votre nom dans theme.config.js ou modifiez le footer.  
1. Mettez à jour votre nom et l’URL du site pour le flux RSS dans scripts/gen-rss.js.  
1. Mettez à jour les meta tags dans pages/_document.js.  
1. Mettez à jour les articles dans pages/posts/*.md avec votre propre contenu.  
```

### Déployez votre propre version
- Déployez l’exemple en utilisant *Vercel* :

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https://github.com/vercel/nextjs-portfolio-starter&project-name=portfolio&repository-name=portfolio)

##$ Comment l’utiliser
- Exécutez create-next-app avec npm ou Yarn pour initialiser l’exemple :
```bash
npx create-next-app --example blog my-blog
```

ou

```text
yarn create next-app --example blog my-blog
```

Déployez-le dans le cloud avec Vercel (Documentation).
