# Mini_Projet consistant à déployer une application wordpress sur minikube

                                    

- Creation d'un deploiement MySQL avec un 1 réplicat
- Creation d'un service de type clusterIP pour exposer le pod à  l'intérieur du cluster
- Creation d'un deploiement wordpress avec des variables d'environnements pour se connecter à la base de données MySQL 
- Le deploiement devra stocker les données de wordpress sur un volume monté  dans /data au niveau du noeud
- Creation d'un service de type NodePort pour exposer le front-end wordpress à l'exterieur du cluster
- Creation d'un service ingress definissant les rules qui vont permettre d'exposer le site wordpress selon la requete tapée par l'utilisateur
- Mise en place d'une ressource de type HorizontalPodAutoscaler afin d'augmenter, ou de diminuer, automatiquement le nombre de réplicas d'un Deployment en fonction de     l'utilisation du CPU.
