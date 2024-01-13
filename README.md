# Projet_IOT

Notre projet de détecteur de fuite d' eau, basé sur la technologie IoT, représente une réponse cruciale pour la préservation de la ressource vitale qu ' est l' eau. Nous espérons que cette initiative contribuera à atténuer les conséquences des fuites d' eau, assurant ainsi la durabilité de nos écosystèmes et la préservation de cette ressource précieuse.

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/16814b4a-6cf1-4e02-8861-23bffbd12a88)

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/9d50275a-8039-4afd-b143-4099aff49a62)

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/ee2c3dd0-ca58-41cb-a6bd-8463fc966c8f)

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/35313f02-bedb-47bf-adb3-2a0b52a31024)

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/bab0fffd-ecf7-439a-8164-64e693306091)

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/1fbe67b2-d5de-4986-87bb-a456160db17c)
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/7acbaf27-77f9-4f10-9e3b-ea5f6ffa72a1)
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/80006851-4f7f-41ea-8e5e-75a3a9418a6e)
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/bcb73376-a9d0-42d6-9d0f-e14678f1b660)
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/806a3b28-3b4e-417b-9cf9-b9d04ffcd15e)
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/25a44734-fd2f-4806-ba0e-7200dfbdd3c8)

Pour illustrer le fonctionnement du détecteur de fuite simulé, une représentation graphique du 
circuit a été créée à l'aide du logiciel Proteus. L'image ci-dessous présente la disposition des 
composants électroniques discutés précédemment, notamment le POT 3214G-1-103E), l'Arduino 
Uno, le condensateur, l'inducteur, l'afficheur LM016L, le potentiomètre POT-HG, et le capteur 
d'eau supplémentaire.
![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/4a85631f-801d-418e-abb0-7801aaedc82f)
Cette représentation visuelle du circuit permet de mieux comprendre la disposition physique 
des composants et offre une perspective claire sur la manière dont ils interagissent au sein du 
détecteur de fuite simulé. Vous pouvez vous référer à cette image tout au long de la section pour 
une visualisation plus concrète du système

## Fonctionnement de circuit
Le fonctionnement du détecteur de fuite est orchestré par un code Arduino élaboré, conçu pour 
surveiller en continu le capteur de fuite et déclencher une alerte en cas de détection. Le code 
s'articule autour de la bibliothèque LiquidCrystal pour la gestion de l'afficheur LCD et de Wire 
pour les communications I2C.

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/6f84746c-7d7e-433d-8b1f-53327bf44992)

Le détecteur commence son processus en affichant le message "Detector Start" sur l'écran 
LCD, signifiant le début du cycle de détection.

![image](https://github.com/AbdellahiDah/Projet_IOT/assets/99772783/5343236b-1382-4d60-89cf-8638a155e15c)

Ce script Python établit une communication bidirectionnelle entre une Raspberry Pi et un 
Arduino via le protocole I2C. 
La Raspberry Pi envoie une requête périodique à l'Arduino, récupère les données reçues, 
extrait la valeur associée, et l'affiche à des fins d'exemple. De plus, le script est conçu pour envoyer 
une notification à une API (fonction sendToAPI()) après chaque itération de la boucle, illustrant 
ainsi un système complet où les incidents détectés par l'Arduino peuvent déclencher des actions 
supplémentaires, telles que des notifications vers une application mobile via une API externe. Ce 
processus permet de garantir une compréhension globale du fonctionnement du système, de la 
détection des fuites par l'Arduino à la notification des utilisateurs par le biais de l'API connectée à 
l'application mobile
