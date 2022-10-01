## Testing our new Navio based architecture

<div style="text-align: center;"><img src="/images/2021-10-08_colibri.jpg" alt="" width="60%"/></div>

<!-- A la suite de difficultés rencontrées sur Condor pour maintenir une architecture robuste aux vibrations, nous avons décidé de passer sur une carte Navio qui est dédiée aux UAV.
Cette carte comporte tout un tas de capteurs et réalise la fusion de données pour permettre d'accéder aux données corrigées.
Encore quelques améliorations doivent être faites comme en atteste la photo ci-dessus ! Le drone a fini dans un arbre car la connexion avec la station sol a été perdue. -->

Following the difficulties encountered on Condor to maintain a vibration resilient architecture, we decided to switch to a Navio board which is a drone controller for Raspberry Pi.
This board has (or can be connected  to) many sensors, it performs data fusion and it provides corrected estimation of the state of the UAV.
Still, some improvements need to be made, as the picture above suggests! The drone ended up in a tree because of a loss of signal with the ground station.
