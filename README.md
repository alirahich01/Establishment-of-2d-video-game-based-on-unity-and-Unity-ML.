
# Project Title
  Ce référentiel contient trois implémentations différentes d'un agent de jeu de paddle utilisant l'algorithme PPO (Proximal Policy Optimization). Chaque implémentation a des objectifs et des résultats spécifiques.

## 1. Implémentation normale avec PPO
  Dans cette implémentation, l'agent apprend à frapper la balle sans bouger excessivement. L'objectif est d'apprendre à frapper la balle tout en évitant de simplement la suivre. L'agent est entraîné à l'aide de l'algorithme PPO avec des paramètres spécifiés dans le fichier config.yaml. La formation est basée sur la récompense extrinsèque et dure 1 million d'étapes.

#### Résultats :

  L'agent a montré une capacité croissante à frapper la balle de manière cohérente, ce qui est réaliste et prometteur.
  La récompense cumulée a augmenté constamment au cours de l'entraînement.
  La durée des épisodes a augmenté, ce qui indique une amélioration.
## 2. Implémentation du self-play compétitif
  Dans cette implémentation, le self-play compétitif est introduit pour former un agent compétitif. Les palettes sont marquées avec des identifiants d'équipe différents. L'objectif est d'apprendre à être compétitif et à explorer de nouvelles stratégies. L'agent est entraîné à l'aide de l'algorithme PPO avec des paramètres spécifiés dans le fichier config.yaml. La formation est basée sur la récompense extrinsèque et dure 1 million d'étapes.

#### Résultats :

  L'agent a développé des stratégies compétitives, mais a du mal à frapper la balle de manière cohérente.
  La récompense cumulée a initialement augmenté, puis a diminué.
  La durée des épisodes a diminué.
## 3. Implémentation combinée
  Dans cette implémentation, les deux méthodes précédentes sont combinées. Les 500 000 premières étapes utilisent l'approche normale avec PPO, puis les 500 000 étapes suivantes utilisent l'auto-jeu compétitif. L'objectif est de frapper la balle de manière fiable tout en conservant des mouvements intéressants. L'agent est entraîné à l'aide de l'algorithme PPO avec des paramètres spécifiés dans le fichier config.yaml. La formation est basée à la fois sur la récompense extrinsèque et l'auto-jeu compétitif, et dure 1 million d'étapes.

#### Résultats :

  L'agent a réussi à frapper la balle de manière fiable et avec des mouvements intéressants.
  La récompense cumulée a augmenté constamment tout au long de l'entraînement.
  La durée des épisodes a augmenté constamment.
En conclusion, l'implémentation combinée a produit les meilleurs résultats, avec un agent capable de frapper la balle de manière plus fiable et compétitive tout en conservant des mouvements intéressants. Vous pouvez trouver les détails de chaque implémentation dans notre Repositories

## 4. Conclusion
  l'implémentation combinée de l'agent de jeu de paddle utilisant l'algorithme PPO se démarque en produisant les meilleurs résultats. En combinant l'approche normale et le self-play compétitif, l'agent parvient à frapper la balle de manière fiable, tout en conservant des mouvements intéressants et compétitifs. Cette approche hybride démontre l'importance de combiner différentes techniques pour maximiser les performances des agents de jeu.
  
## 5. Références :
1-https://openai.com/research/openai-baselines-ppo
2-https://openai.com/research/competitive-self-play
3-Introduction to ML-Agents in Unity and Virtual Environments(Video Youtube)
4-https://github.com/Unity-Technologies/ml-agents
5-https://thomassimonini.medium.com/an-introduction-to-unity-ml-agents-with-hugging-face-efbac62c8c80
6-https://www.youtube.com/watch?v=6WcBis699zI
