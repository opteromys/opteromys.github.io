## Our new simulator

<div style="text-align: center;"><img src="/images/2020-07-17_simulator.jpg" alt="" width="60%"/></div>

<!-- Le principal frein au développement de nos drones est la nécessité de tester son fonctionnement pour valider le comportement d'algorithmes.
Pour faciliter le développement nous avons donc entrepris de coder un simulateur physique.
Nous sommes parti des équations régissant la dynamique d'une voile de parapente pour écrire un code permettant de simuler l'évolution du drone dans son environnement.
Ce simulateur permet de simuler l'exécution de l'intégralité des codes du drone en remplaçant les capteurs par des briques élémentaires qui récupèrent les données du simulateur.
Au départ codé en Python, nous sommes passés sur une implémentation en C++ pour gagner en vitesse d'exécution. -->

The main limitation to the development of our drones is the need to test and verify each of their functionalities, before finally validating the behavior of our algorithms under development.
In order to facilitate  future developments, we undertook to implement a simulator.
We started from the equations governing the dynamics of a paragliding wing to write a code that simulates the evolution of the drone in its environment.
This simulator allows us to simulate the execution of the whole code of the drone by replacing the sensors by programs which recover the data of the simulator.
This approach is known as *software-in-the-loop*.
Initially coded in Python, we switched to a C++ implementation to gain in execution speed.
