# harddrive
Some informations about hard drive to avoid crash

commande : **smartctl -i /dev/sdx** donne la marque, le modele, le numero de série, la capacité du disque dur, le firmware.

**smartctl -s on -o on -S on /dev/sdx**

**smartctl -H /dev/sdx** qui doit retourner passed.
    
**smartctl -c /dev/sdx**  qui donne des informations mais je ne sais à quoi sert cette commande

**smartctl -t short /dev/sdx** On ne peut pas suivre la progression de cette commande. 

**smartctl -t long /dev/sdx** peut prendre PLUSIEURS HEURES. Cela se lance le soir et on regarde les résultats le matin.

Pour voir le résultat de ces deux dernières commandes il faut : **smartctl -l selftest /dev/sdx**
