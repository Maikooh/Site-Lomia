<a name="french-version"></a>

# Développement web : Site web Lomia

> 🇬🇧 [English version below](#english-version) | 🇫🇷 Version française

Site Lomia est un site web constitué d’un ensemble de pages HTML/CSS dédiées à la présentation visuelle de projets, créations graphiques et galeries d’images.
Ce projet met en avant différents univers visuels organisés en catégories (portraits, mockups, stickers, etc.) au travers d’un site statique entièrement customisé dans le cadre de l'apprentissage du développement web.

## 📁 Structure du projet

```
Site-Lomia/
│
├── index.html                       # Page d'accueil du site
├── img/                             # Images globales
|
├── css/                             # Styles principaux du site
│   ├── base.css                     # Styles de base (typographies, couleurs...)
│   ├── components.css               # Composants réutilisables
│   └── layout.css                   # Mise en page générale
│
├── article/                         # Pages "article" avec leurs styles
│   ├── img/                         # Images associées aux pages article
│   ├── article.css
│   ├── draco.html
│   ├── karmeilet_design.html
│   ├── ratatouille_design.html
│   ├── Ratatouille.html
│   ├── spip.html
│   └── template.html                #template initiale pour les articles
│
│
├── galerie/                         # Toutes les pages de galeries
│   ├── Mockup/                      # Images mockup
│   ├── Portrait/                    # Images portraits
│   ├── Stickers/                    # Images stickers
│   ├── Tout/                        # Images de la galerie générale
│   │
│   ├── divers.css                   #css de la galerie générale
│   ├── divers.html
│   ├── galerie1.css
│   ├── galerie2.css
│   ├── mockup.html                 #css associé -> galerie 2
│   ├── portrait.html               #css associé -> galerie 2
│   └── stickers.html               #css associé -> galerie 1
│
|
│
├── portfolio/                       # Section portfolio
│   │
│   ├── solomon/                         # Dossier du portfolio Solomon
│   │   ├── img/                         # Images de Solomon
│   |   ├── solomon.css
│   |   └── solomon.html
│   |
│   └── tsiki/                           # Dossier du portfolio Tsiki
│       ├── img/                         # Images Tsiki
│       ├── tsiki.css
│       └── tsiki.html
│
├── .gitignore
└── README.md

```

## Installation

Simple lecture ici :  
➡️ [https://maikooh.github.io/projet/devweb/lomia.html](https://maikooh.github.io/projet/devweb/lomia.html)

#### 1. Télécharger le projet

Deux solutions possibles :

```bash
git clone https://github.com/Maikooh/Site-Lomia.git
```

ou alors :

Téléchargez le projet au format `.zip` depuis le dépôt GitHub :  
➡️ [https://github.com/Maikooh/Site-Lomia](https://github.com/Maikooh/Site-Lomia)

Décompressez le fichier `.zip`

### 2. Lancer le site

Ouvrir **index.html** dans un navigateur.

## Technologies utilisées

- **HTML5**
- **CSS3**

## Contenu & Fonctionnalités

- Galeries d'images (mockups, portraits, stickers, divers)
- Pages dédiées pour certains projets visuels
- Styles modulaires (base, components, layout)

## Développement

### Ajouter une page

**Prenons en exemple un portfolio**

1.  Créer un fichier HTML : **exemple.html**
2.  Ajouter le CSS associé: **exemple.css**
3.  Ajouter les images au bon dossier: **img_exemple**
4.  Mettre à jour les liens dans `index.html`

```
Site-Lomia/
│
├── index.html
├── img/
├── css/
├── article/
│
├── galerie/
|
├── portfolio/
│   │
│   ├── solomon/
│   ├── tsiki/
|   |
│   └── portfolio_exemple/    #dossier du portfolio exemple
│       ├── img_exemple/      # Images du portfolio exemple
│       ├── exemple.css       # CSS de la page exemple
│       └── exemple.html      # HTML de la page exemple
│
├── .gitignore
└── README.md

```

Puis dans **index.html** ajouter dans la section correspondante :

```html
<!-- Section Portfolio -->
<div
  class="card"
  style="--bg: url('path de l'image d'illustration');    
         --text-color : #couleur du texte ;  
         --stroke-color:#couleur du contour de texte;"
>
  <a
    href="./portfolio/portfolio_exemple/exemple.html (path)"
    target="_blank"
    class="card-link"
  >
    <h3>TITRE</h3>
    <p>texte de contenu de présentation</p>
  </a>
</div>
```

## Auteur

- **Fadli Aaron** - [LinkedIn](https://www.linkedin.com/in/aaron-fadli/) | [GitHub](https://github.com/Maikooh) | [Site web](https://maikooh.github.io/)

## Licence

CC-BY-NC - Fadli Aaron | Master MECEN 2025-2026

L'utilisation ou diffusion du contenu de ce projet est autorisé sous réserve de mentionner l'auteur et la source. Toute exploitation commerciale requiert une autorisation écrite.

Projet réalisé dans le cadre du [Master Économiste d'entreprise](https://mecen.univ-tours.fr/) de l' [Université de Tours](https://www.univ-tours.fr/).

## Support

Pour toute question ou problème :

- Ouvrir une issue sur GitHub
- [Me contacter par mail](mailto:aaron.fadli@etu.univ-tours.fr)

---

<a name="english-version"></a>

# Web Development: Lomia Website

> 📝 _This README was translated with AI assistance_  
> 🇫🇷 [Version française ci-dessus](#french-version) | 🇬🇧 English version

Lomia Website is a static HTML/CSS project structured around visual showcases, portfolios, and image galleries.
It highlights several artistic universes—portraits, mockups, stickers, and more—through individually designed pages.
This website was created as part of web development learning.

```
Site-Lomia/
│
├── index.html                       # Main homepage
├── img/                             # Global images
│
├── css/                             # Main styling files
│   ├── base.css                     # Base styles (typography, colors, reset)
│   ├── components.css               # Reusable UI components
│   └── layout.css                   # General layout rules
│
├── article/                         # Article-like pages
│   ├── img/                         # Images used by articles
│   ├── article.css
│   ├── draco.html
│   ├── karmeilet_design.html
│   ├── ratatouille_design.html
│   ├── Ratatouille.html
│   ├── spip.html
│   └── template.html                # Base template for new articles
│
├── galerie/                         # Image gallery pages
│   ├── Mockup/                      # Mockup gallery images
│   ├── Portrait/                    # Portrait gallery images
│   ├── Stickers/                    # Stickers gallery images
│   ├── Tout/                        # General gallery images
│   │
│   ├── divers.css
│   ├── divers.html
│   ├── galerie1.css
│   ├── galerie2.css
│   ├── mockup.html                  # Uses galerie2.css
│   ├── portrait.html                # Uses galerie2.css
│   └── stickers.html                # Uses galerie1.css
│
├── portfolio/                       # Portfolio section
│   │
│   ├── solomon/                     # Solomon project
│   │   ├── img/
│   │   ├── solomon.css
│   │   └── solomon.html
│   │
│   └── tsiki/                       # Tsiki project
│       ├── img/
│       ├── tsiki.css
│       └── tsiki.html
│
├── .gitignore
└── README.md
```

## Installation

View it here :  
➡️ [https://maikooh.github.io/projet/devweb/lomia.html](https://maikooh.github.io/projet/devweb/lomia.html)

#### 1. Dowload the Project

Two possible solutions :

```bash
git clone https://github.com/Maikooh/Site-Lomia.git
```

ou alors :

Download the project as a `.zip` file from the GitHub repository :  
➡️ [https://github.com/Maikooh/Site-Lomia](https://github.com/Maikooh/Site-Lomia)

Unzip the `.zip` file.

### 2. Lauch the website

Open **index.html** in a browser.

## Technologies Used

- **HTML5**
- **CSS3**

## Content & Features

- Image Galleries (mockups, portraits, stickers, miscellaneous)
- Dedicated pages for specific visual projects
- Modular Styles (base, components, layout)

## Developpement

### Adding a New Page

**Let's take a portfolio as an example**

1. Create an HTML file: **example.html**

2. Add the associated CSS: **example.css**

3. Add the images to the correct folder: **img_example**

4. Update the links in `index.html`

```
Site-Lomia/
│
├── index.html
├── img/
├── css/
├── article/
│
├── galerie/
|
├── portfolio/
│   │
│   ├── solomon/
│   ├── tsiki/
|   |
│   └── portfolio_example/    # Example portfolio folder
│       ├── img_example/      # Images for example portfolio
│       ├── example.css       # CSS for example page
│       └── example.html      # HTML for example page
│
├── .gitignore
└── README.md

```

Then, in **index.html** add the following in the corresponding section :

```html
<!-- Section Portfolio -->
<div
  class="card"
  style="--bg: url('path to illustration image');    
         --text-color : #text-color ;  
         --stroke-color:#text-outline-color;"
>
   
  <a
    href="./portfolio/portfolio_exemple/exemple.html (path)"
    target="_blank"
    class="card-link"
  >
       
    <h3>TITLE</h3>
       
    <p>presentation content text</p>
     
  </a>
</div>
```

## Author

- **Fadli Aaron** - [LinkedIn](https://www.linkedin.com/in/aaron-fadli/) | [GitHub](https://github.com/Maikooh) | [Site web](https://maikooh.github.io/)

## Licence

CC-BY-NC - Fadli Aaron | Master MECEN 2025-2026

The use or distribution of the content of this project is authorized, provided the author and source are mentioned. Any commercial exploitation requires written authorization.

Project carried out as part of the [Master Économiste d'entreprise](https://mecen.univ-tours.fr/) (Business Economist Master's Degree) at the [University of Tours](https://www.univ-tours.fr/).

## Support

For any questions or issues:

- Open an issue on GitHub
- [Mail me](mailto:aaron.fadli@etu.univ-tours.fr)

---
