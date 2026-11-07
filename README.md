# Paris Grand Jeu

Application de grand jeu urbain dans Paris : les équipes s'inscrivent en scannant un QR code, suivent les itinéraires, débloquent les énigmes sur place (GPS ou balise QR) et écrivent au Maître du jeu. L'organisateur suit tout en direct depuis la régie.

- **Joueurs** : `https://yoyo-fait-son-show.github.io/grand-jeu-paris/`
- **Régie** : `https://yoyo-fait-son-show.github.io/grand-jeu-paris/#regie` (protégée par un code)
- **Démo** avec équipes simulées : `https://yoyo-fait-son-show.github.io/grand-jeu-paris/demo/`

## Installation (une seule fois)

1. Créer un projet gratuit sur [Supabase](https://supabase.com).
2. Dans le projet : **SQL Editor → New query**, coller le contenu de `setup.sql` (fourni à part, pas dans ce dépôt public), puis **Run**.
3. Renseigner l'adresse du projet et sa clé publique (*publishable* ou *anon*) dans `config.js`. Ne jamais y mettre la clé secrète (*secret* ou *service_role*).
4. Ouvrir la régie (`#regie`) et choisir le code secret de l'organisateur.

## Organiser une partie

- **Parcours** : ajouter, modifier ou déplacer les étapes depuis la régie. Les énigmes d'exemple sont publiques (elles servent aussi à la démo) : écrivez les vôtres pour une vraie partie.
- **Imprimer les QR codes** (onglet Parcours) : le QR d'inscription à poser au départ, et une balise par étape à coller sur place. Scanner la balise débloque l'énigme, même sans GPS.
- **Pendant la partie** : carte des équipes en direct, alertes (équipe bloquée depuis 10 min, hors ligne depuis 3 min), questions des équipes, messages à une équipe ou à toutes, pause, points bonus, validation manuelle.
- **Nouvelle partie** : onglet Diffusion → Réglages → effacer les équipes (le parcours est conservé).

## Bon à savoir

- Les réponses et l'emplacement exact des étapes restent sur le serveur : les téléphones ne voient que la zone de recherche, puis l'énigme une fois sur place.
- Sur iPhone, le GPS s'arrête quand l'écran se verrouille : demandez aux équipes de garder l'écran allumé pendant la marche.
- Un projet Supabase gratuit se met en veille après une semaine sans activité. Il se réactive depuis le tableau de bord Supabase.

## Crédits

Fond de carte © contributeurs [OpenStreetMap](https://www.openstreetmap.org/copyright) · Contours des arrondissements : Ville de Paris (ODbL) · [Leaflet](https://leafletjs.com) · [qrcodejs](https://github.com/davidshimjs/qrcodejs).
