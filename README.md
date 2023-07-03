# ThailandSwiperSlide
#####Caroussel avec la function swiper slide en utilisant HTML-CSS-Javascript

Le principe de "swiper slide" est lié à une bibliothèque populaire appelée Swiper.js, qui permet de créer facilement des carrousels et des galeries d'images interactives.

Lorsque vous utilisez Swiper.js, vous devez créer une structure HTML pour votre carrousel en utilisant des éléments <div> avec la classe "swiper-container" pour le conteneur principal et des éléments enfants avec la classe "swiper-slide" pour chaque diapositive.
1.Html
```Html
<div class=" swiper mySwiper">
    <div class="swiper-wrapper">
       <div class="swiper-slide">
        <img src="images/1.jpg" alt="buddha">
        <div class="center">
            <h5>Bouddha de Thailande</h5>
            <P> Le Grand Bouddha de Thaïlande (Phra Buddha Maha Nawamin ou Mahaminh Sakayamunee Visejchaicharn) est une statue de Bouddha 
                en ciment doré haute de 92 mètres. Plus haute statue de Thaïlande, elle est en 2022 la 9e plus haute statue du monde.
            </P>
        </div>
       </div>
```
2.Javascript
Le Swiper est une bibliothèque JavaScript populaire utilisée pour créer des carrousels, des diaporamas et des galeries d'images interactives dans les applications web et mobiles. Il fournit une solution simple et flexible pour parcourir et naviguer entre différents éléments, tels que des images, des cartes, des articles, etc.

Le Swiper facilite la mise en place de fonctionnalités de glissement (swiping), de pagination, de navigation précédent/suivant et d'autres interactions tactiles pour améliorer l'expérience utilisateur. Il prend également en charge la prise en charge du clavier et des gestes de souris pour une expérience plus accessible.

Le Swiper est souvent utilisé dans les sites Web et les applications qui nécessitent une présentation visuelle attrayante et une interaction fluide avec les contenus présentés. Il offre des options de personnalisation étendues, telles que le contrôle de la vitesse de transition, la pagination personnalisée, les effets de transition, les événements de rappel, etc.

En résumé, le Swiper en JavaScript est une bibliothèque qui permet de créer facilement des carrousels et des galeries d'images interactives avec des fonctionnalités de glissement et de navigation. Il offre une expérience utilisateur améliorée et est largement utilisé dans le développement d'applications web et mobiles.
```Javascript
const swiper = new Swiper(".mySwiper",{
    // Initialise un nouveau carrousel Swiper en utilisant la classe "mySwiper" comme sélecteur
   effect:"coverflow",// Utilise l'effet de coverflow pour la transition entre les diapositives
   grabCursor:true,// Change le curseur en une main lorsqu'il survole le carrousel
   centeredSlider:true,// Centre la diapositive active dans le carrousel
   loop:true,//Permet de faire une boucle infinie du carrousel


   coverflowEffect:{
    rotate:60,// L'angle de rotation des diapositives en mode coverflow
    stretch:0,// L'espacement horizontal entre les diapositives en mode coverflow
    slidesshadow:true // Active les ombres portées pour les diapositives en mode coverflow
     
     },
     slidesPerView:"auto",// Définit le nombre de diapositives visibles par vue, "auto" signifie autant de diapositives que possible
     pagination:{
        el:".swiper-pagination"// Sélectionne l'élément avec la classe "swiper-pagination" pour afficher la pagination
         
         }   
})
```
