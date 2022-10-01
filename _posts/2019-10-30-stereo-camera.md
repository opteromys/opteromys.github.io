## Testing the Intel Realsense stereo camera

<!-- ![](/images/2019-10-30-stereo-camera.jpg) -->
<div style="text-align: center;"><img src="/images/2019-10-30-stereo-camera.jpg" alt="" width="60%"/></div>

<!-- Recently we acquired an Intel Realsense camera to integrate it on our drone.
This camera uses both a stereo technology and an infrared sensor to get depth information.
This project has  -->

<!-- Nous avons récemment fait l'acquisition d'une caméra Intel Realsense pour l'intégrer sur notre drone.
Cette caméra utilise une technique stéréo et un capteur infrarouge pour calculer la profondeur aux objets imagés.
Notre but est de savoir à quel point ce capteur peut être exploité sur notre drone pour obtenir de l'information sur son environnement.
Cela pose de nombreuses questions, notamment comment traiter la grande quantité de données collectées à bord sachant qu'actuellement le drone utilise une Raspberry Pi. -->

We recently acquired an Intel Realsense camera to supplement our drone with precise landing -- and possibly sense & avoid -- capabilities.
This camera uses a stereo technique and an infrared sensor to get depth information of the imaged objects.
Our goal is to know to what extent this sensor can be used on our drone to obtain information on its environment.
Its integration within the drone raises many questions, including how to process the large amount of data collected on board knowing that the drone currently uses a Raspberry Pi.
