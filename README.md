# Denoising

L'objectif est d'estimer à partir du signal bruité le signal de voix. Pour cela, 3 approches ont été réalisés:

- Un "Dumb model" réalisé à parti d'un modèle Unet sur la forme d'onde disponible dans le dossier ""

- Une méthode "WaveUnet" basé sur la forme d'ondes  disponible dans le dossier ""

- Une méthode Unet basé sur le spectrogramme disponible dans le dossier "method_spectro ""

# Analyse des résultats

Pour réaliser notre analyse, 2 mesures ont été prises en compte : 
- Le PESQ (Perceptual Evaluation of Speech Quality): L'objectif d'un denoising est de maximiser cette valeur pour estimer au mieux le signal de voix.
- Le STOI (Short Term Objective Intelligibility) : l'objectif d'un denoising est d'enlever le bruit sans avoir un impact significatif sur cette métrique pour que la voix reste intelligible.

Par ailleurs, ces 2 métriques sont combinés à une analyse manuelle "à l'oreille" de nos résultats pour comprendre quelles sont les points forts et points faibles de chaque modèle.