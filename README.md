> MalhoStephane_3_27032021
 # Ohmyfood 
> Ceci est mon deuxième projet de cours Openclassrooms.
> Le projet porte en particulier sur l'utilisation se SASS et sur les animations CSS3.

## Informations générales
Développer un site proposant le menu de 4 grands restaurants Parisiens.
* Le développement devra se faire en CSS, sans JavaScript.
* Aucun framework ne devra être utilisé, en revanche l’utilisation de SASS est conseillée.
* Aucun code CSS ne devra être appliqué via un attribut style dans une balise HTML.

## Captures d'écran
 [Capture d'écran] (./assets/images/screen/menu.png)

## Les prérequis 
* apprendre à utiliser SASS 
* apprendre les animations en CSS3

## Les technologies
* HTML5
* CSS3
* SASS au format SCSS
* NPM 

## Exemples de code
```css
#entries {
  @include lazy(4,0);
}
#main-courses {
  @include lazy(3,0.6);
}
#desserts {
  @include lazy(3,1.2);
}
```
```css
@mixin lazy($limit,$delay) {
    @for $i from 1 through $limit {
        article:nth-of-type(#{$i}) {
          animation: slide-top 1s ease-out ($delay + (0.2s * $i)) both;
        }
      }
}
// ANIMATION DELAY FOR LAZY LOADING //
```

## Caractéristiques

Ce site est un prototype crée à partir d'une maquette mobile, le format tablette et desktop à été adapté par le développeur.(moi ^^)

### Fonctionnalité 
* une page principale et quatres pages pour les menus de restaurants
* structure du site mobile first 
* format responsive 
* animation au hover sur les articles de menu avec check icon (au hover)
* loading spinner sur la page principale
* les boutons changent d'apparansse au survol


## Statut
Le projet est: terminée 
Bien qu'il ne soit pas fonctionnel, les livrables ont été respectés, 

## Inspiration
Projet inspiré de cours https://openclassrooms.com
source supplémentaire https://developer.mozilla.org/
validé https://validator.w3.org/





