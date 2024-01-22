# Denoising

L'objectif est d'estimer à partir du signal bruité le signal de voix. Pour cela, 3 approches ont été réalisées:

- Un "Dumb model" réalisé à parti d'un modèle Unet sur la forme d'onde disponible dans le dossier "method_signal"

- Une méthode "WaveUnet" basée sur la forme d'ondes disponible dans le dossier "method_waveUnet" (cf D. Stoller et Al., WAVE-U-NET: A MULTI-SCALE NEURAL NETWORK FOR END-TO-END AUDIO SOURCE SEPARATION, ISMIR 2018)

- Une méthode Unet basée sur le spectrogramme disponible dans le dossier "method_spectro" (cf A. Jansson et Al., SINGING VOICE SEPARATION WITH DEEP U-NET CONVOLUTIONAL NETWORK, ISMIR 2017 )

# Analyse des résultats

Pour réaliser notre analyse, 2 mesures ont été prises en compte :
- Le PESQ (Perceptual Evaluation of Speech Quality): L'objectif d'un denoising est de maximiser cette valeur pour estimer au mieux le signal de voix.
- Le STOI (Short Term Objective Intelligibility) : l'objectif d'un denoising est d'enlever le bruit sans avoir un impact significatif sur cette métrique pour que la voix reste intelligible.

Par ailleurs, ces 2 métriques sont combinées à une analyse manuelle "à l'oreille" de nos résultats pour comprendre quelles sont les points forts et points faibles de chaque modèle.