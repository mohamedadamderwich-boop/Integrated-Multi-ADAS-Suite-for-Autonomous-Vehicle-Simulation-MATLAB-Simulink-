# Integrated Multi-ADAS Suite for Autonomous Vehicle Simulation (MATLAB/Simulink)
## Description : 
Conception d'une architecture modulaire en boucle fermée pour un véhicule autonome (Modèle Bicycle), incluant le freinage d'urgence (AEB), le maintien de voie (LKA), l'évitement d'obstacle (ESA) et la gestion intelligente de la visibilité.
## Architecture Système:

Contrôle Longitudinal ($v$) : Arbitrage entre la vitesse de croisière (ACC) et la sécurité (AEB) via le calcul du TTC (Time-To-Collision).

Contrôle Latéral ($\delta$) : Asservissement de direction pour le maintien de voie (LKA) et bifurcation dynamique vers une voie d'évitement (ESA).
## Modélisation Mathématique

Les équations de mon Subsystem :

$$\dot{x} = v \cdot \cos(\theta)$$

$$\dot{y} = v \cdot \sin(\theta)$$

$$\dot{\theta} = \frac{v}{L} \cdot \tan(\delta)$$

Où $L$ est l'empattement et $\delta$ l'angle de braquage.
