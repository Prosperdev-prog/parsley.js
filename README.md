# parsley.js
validation de formulaire ynamique avec ajax
Ce projet utilise **Parsley.js** comme outil dynamique pour la validation des formulaires. Parsley.js est une bibliothèque JavaScript qui facilite la validation des formulaires en fournissant des fonctionnalités robustes et faciles à utiliser.

Installation

Pour utiliser Parsley.js dans votre projet, vous pouvez l'installer via npm ou inclure directement le fichier JavaScript dans votre projet.

 Via npm :
npm install parsleyjs
Via CDN :
Vous pouvez également inclure Parsley.js directement depuis un CDN :
<script src="https://cdnjs.cloudflare.com/ajax/libs/parsley.js/2.9.2/parsley.min.js"></script>

Utilisation
Pour activer la validation des formulaires avec Parsley.js, ajoutez simplement l'attribut data-parsley-validate à votre balise <form>. Voici un exemple :

<form id="myForm" data-parsley-validate>
    <input type="text" name="username" required data-parsley-minlength="3" />
    <input type="email" name="email" required />
    <button type="submit">Soumettre</button>
</form>
Ensuite, initialisez Parsley.js dans votre script JavaScript :

$(document).ready(function() {
    $('#myForm').parsley();
});

Fonctionnalités
Validation en temps réel des champs de formulaire.
Messages d'erreur personnalisables.
Support pour les validations personnalisées.
Intégration facile avec jQuery.
