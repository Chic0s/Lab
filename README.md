<h2 class="center">Création d'un lab</h2>

<h3 style="font-style: italic;">Ce laboratoire permettra de faire de créer un RDP et de pouvoir faire différents tests..</h3>

<p>
Il existe des solutions gratuites pour émuler un OS. (Virtual Box, VMware)
Pour analyser un malware dans un environnement windows, il est possible d'utiliser https://any.run. 
</p>

<h3 align="center">Comment procéder à la création du Lab dans un milieu personnel.</h3>

<h2>Choix du matériel</h2>

<p> 
Dans un premier temps, il faut choisir un serveur en fonction des différents critères. 
</p>

<h3>Choix du serveur</h3>

<ul>
    <li>Processeur</li>
    <li>RAM (Attention la ram serveur est différentes de la RAM classique)</li>
    <li>L'espace disque, notamment le nombre de slots disponibles.</li>
    <li>Définition de l'OS qui sera installé</li>
</ul>

<p>
Il est important de faire attention au coût du matériel, ce qui m'a freiné à prendre un serveur neuf. 

Je me suis donc redirigé sur Ebay pour prendre un serveur reconditionné. 

J'ai pu trouver un serveur R620, avec deux processeurs E5-2670, 32 GB de ram et 8 slots pour disque dur. ~ 150€
</p>


![dell-poweredge-r620-2-x-e5-2630-v2-six-core-xeon-2](https://user-images.githubusercontent.com/96829109/188813588-1a976536-e97c-4be3-b09d-2261ae2fcd72.jpg)

<p> 
Il existe différents types de serveurs : tour, rack ... 

Personnellement j'ai choisi un serveur rack car mon objectif final reste la création d'une baie. 
</p>

<h3>Choix du switch</h3>

<p>
Je souhaite isoler mon serveur sur un VLAN pour que mes "invités" ou personnes malvaillantes ne puissent pas accéder à mon serveur en wifi. 

J'ai donc opté pour l'utilisation d'un switch. 

Grâce à un camarade, j'ai pu récupérer un switch ayant un débit de 100 MB. 
</p>

![th-2315720400](https://user-images.githubusercontent.com/96829109/188817221-7237f042-5b31-4ac5-9a9b-7003af8cbaf1.jpg)

<p>
Image illustratice
</p>

<h2 align="center"> Configuration du serveur </h2>

<h3>Mise à jour du BIOS</h3>

<p>
Pour mettre à jour le BIOS, j'ai récupérer le numéro du série du serveur DELL et je me suis rendu sur le site officiel de DELL. 
J'ai récupérer l'iso puis je l'ai mis sur une clée USB à l'aide de RUFUS. 

A la suite de cette mise à jour, j'ai pu activer le port IDRAC pour configurer à distance le serveur. (ip par défaut: 192.168.0.200)
</p>

