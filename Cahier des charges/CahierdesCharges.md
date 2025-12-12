Cahier des charges — Projet RADARDUINO
1. Présentation du projet

Le RADARDUINO est un projet réalisé en collaboration entre AKBAB Younisse et Théo Lassaunière dans le cadre de notre travail Arduino.
L’objectif principal est de concevoir un radar fonctionnel, capable de détecter un objet en mouvement, de mesurer sa vitesse, puis d’afficher cette vitesse en temps réel sur un écran.

Le système repose sur l’utilisation d’un capteur de distance, d’un servomoteur permettant une rotation contrôlée, ainsi que d’un écran pour l’affichage des informations.

2. Fonctionnement général

Le radar utilise un capteur de distance pour repérer un objet à deux positions distinctes dans l’espace, séparées par un court intervalle de temps.
À partir de ces deux mesures de distance, il calcule la vitesse de déplacement de l’objet grâce à la formule :

<img width="234" height="79" alt="image" src="https://github.com/user-attachments/assets/44e31930-1af2-4b3d-b61a-32e29d407355" />

Le système compare ensuite cette vitesse à une vitesse limite programmée dans le code.
Si l’objet dépasse ce seuil, le Radarduino signale le dépassement et affiche la vitesse mesurée sur l’écran.

3. Composants nécessaires

   3.1. Capteur de distance
  - Sert à mesurer la distance entre le radar et l’objet détecté.

  - Plusieurs capteurs ont été testés (VL53L0X, Lidar Lite v3HP, CQRobot Microwave, TF Mini S) afin de trouver celui offrant la meilleure précision.

  3.2. Servomoteur
     - Permet au capteur de tourner sur lui-même pour couvrir un angle défini.

     - Assure une balayage de la zone à analyser.

  3.3. Écran 2.8" TFT LCD
    - Affiche la vitesse mesurée et l’état du radar (détection, dépassement de vitesse, valeurs en temps réel).

  3.4. Carte Arduino
    - Cœur du système : reçoit les données du capteur, effectue les calculs et pilote l’écran et le servomoteur.

4. Objectifs du projet
   4.1. Objectifs techniques
    - Concevoir un radar fonctionnel capable de :
    - mesurer des distances précises,
    - calculer la vitesse d’un objet en mouvement,
    - détecter les dépassements de limite de vitesse,
    - afficher les informations sur un écran en temps réel.
    - Intégrer tous les composants dans une structure solide conçue en modélisation 3D.
    - Obtenir un montage stable, cohérent et résistant.

  4.2. Objectifs organisationnels
  
      - Respecter les délais imposés durant les 8 semaines de projet.
      - Répartir les tâches équitablement entre les membres du binôme.
      - Travailler de manière autonome tout en assurant une bonne coordination de groupe.
      - Adapter le projet face aux contraintes techniques (changements de capteurs, compatibilités, etc.).

5. Contraintes

Contraintes techniques :

- Choisir un capteur suffisamment précis pour calculer la vitesse.
- Assurer une rotation fluide du servomoteur.
- Gérer la compatibilité entre les différents composants (bibliothèques Arduino, alimentation, connexions).

Contraintes matérielles :

- Respecter les composants disponibles au collège/lycée.
- Adapter la modélisation 3D au matériel choisi.

Contraintes temporelles :

- Réalisation complète en 8 semaines.

Contraintes rencontrées :

- Difficultés avec l’écran TFT LCD, qui n’a pas été entièrement fonctionnel.

6. Résultat attendu

À la fin du projet, le RADARDUINO doit être capable de :

- détecter un objet en mouvement,
- calculer sa vitesse,
- comparer cette vitesse à un seuil programmé,
- afficher les résultats sur un écran,
- effectuer un balayage automatique grâce au servomoteur,
- être intégré dans une structure imprimée en 3D.

À la fin du projet, l’ensemble des résultats attendus ont été atteints : le Radarduino fonctionne conformément aux objectifs fixés et respecte les contraintes imposées.
