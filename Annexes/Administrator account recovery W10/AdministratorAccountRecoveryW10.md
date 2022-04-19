# Administrator Account Recovery W10

1. Booter sur l'image disponible ici : https://sourceforge.net/projects/systemrescuecd/
2. Une fois le clavier configuré, lister les partitions : ```ls```
3. ```mkdir /sda2``` (remplacer sda2 par l'identifiant de la partition W10)
4. ```ntfs-3g /dev/sda2 /sda2``` 
5. ```cd /sda2```
6. ```chntpw -l SAM``` (liste les users de la machine)

## Déverrouillage du compte Admin

7. ```chntpw -u Administrateur SAM``` --> ```2``` (déverrouille le compte Admin)

## Suppression du mot de passe d'un utilisateur

7. ```chntpw -u Administrateur SAM``` --> ```1``` (déverrouille le compte Admin)
