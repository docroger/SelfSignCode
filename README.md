# SelfSignCode
Self signing certificat creator

SelfSignCode 1.4.1
============

by Docno - 2023
windows 10/11 : 32/64 bits
DonationWare

Le mode DEMO ne permet de signer que le premier ficher de la liste.

Petit utilitaire qui permet de signer des exe windows avec un certificat personnel.
Regroupe tous les utilitaires nécessaires sans avoir besoin d'installer le sdk windows.

 - capicom.dll
 - cert2spc.exe
 - makecert.exe
 - pvk2pfx.exe
 - pvkimprt.exe
 - signtool.exe

Prêt à fonctionner et super simplifié.

Utilisation 
===========

Générer son propre certificat : onglet certificat.
Remplir les champs nom et mot de passe et choisir une date de validité puis CREER.
Dans le dossier keys les fichiers suivants sont générés :
 - xxxx_cert.cer
 - xxxx_cert.pfx
 - xxxx_cert.pvk
 - xxxx_cert.spc

Avec xxxx = le nom du certificat choisi.
Le fichier pfx peut être transmis à des clients pour être installé sur leur poste. 
Sélectionner le pfx, bouton droit et menu Installer le PFX.
---------------------

Signer des exe/dll/ocx/msi/cab : onglet signer.
En général il faut au préalable activer CAPICOM.DLL (menu options).
Sélectionner le certificat à utiliser.
Puis glisser/déposer les fichiers à signer dans la liste.
Puis SIGNER.

Pour vérifier qu'un fichier est signé,dans l'explorateur de fichiers, faire propriétés.
Un onglet Signature numériques est présent.

Pour finir proprement, faire désactiver CAPICOM.DLL (menu options).

Le programme peut aussi servir à signer avec un certificat acheté auprès d'une autorité de certification.

+++++++++++++++++++++++++++++++++
