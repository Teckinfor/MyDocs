# Comment réécrire le bootloader sur W10
1. Booter sur une image d'installation
2. Aller dans Réparer > Options avancées > Prompt
3. diskpart
4. sel disk 0
5. list vol
6. sel vol X (X = partition FAT32 de 100Mo)
7. assign letter=N:
8. exit
9. N:
10. format N: /FS:FAT32 (va formater toute la partition)
11. bcdboot C:\windows /s N: /f UEFI
12. reboot
