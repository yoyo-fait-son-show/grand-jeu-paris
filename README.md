# Paris Grand Jeu · démo

Démo cliquable d'un grand jeu urbain dans Paris : inscription des équipes par QR code, énigmes, GPS du téléphone, et régie en temps réel avec cinq équipes simulées.

## Essayer

Ouvrez la page publiée par GitHub Pages, puis :

- **Régie** : carte des équipes en direct, fil d'activité, parcours modifiable, messages à toutes les équipes, QR code d'inscription.
- **Joueur** : inscrivez une équipe, activez le GPS (ou touchez la carte pour simuler), répondez aux énigmes.

Liens directs : ajoutez `#inscription` à l'adresse pour arriver sur l'inscription, ou `#balise-pz7k` (code de chaque étape) pour simuler le scan d'une balise sur place.

## Limites de cette version

- Chaque téléphone joue de son côté : il n'y a pas encore de serveur, donc la régie ne voit que les équipes simulées et l'équipe du même téléphone.
- Le Maître du jeu IA est en pause : il a besoin d'un serveur avec une clé API, prévu pour l'app finale.
- Les réponses des énigmes sont lisibles dans le code source. Pour un vrai jeu public, elles devront être vérifiées côté serveur.

## Crédits

- Fond de carte © contributeurs [OpenStreetMap](https://www.openstreetmap.org/copyright) (ODbL), tuiles OpenStreetMap à usage modéré.
- Contours des arrondissements : Ville de Paris, Open Data (ODbL).
- [Leaflet](https://leafletjs.com) (BSD-2) et [qrcodejs](https://github.com/davidshimjs/qrcodejs) (MIT).
