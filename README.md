# opd
#1 task
mkdir lab0
mkdir lab0/drowzee3
mkdir lab0/drowzee3/lickilicky
mkdir lab0/drowzee3/finneon
touch lab0/drowzee3/karrablast
touch lab0/drowzee3/bellossom
mkdir lab0/drowzee3/chimecho
mkdir lab0/drowzee3/venonat
mkdir lab0/grimer7
mkdir lab0/grimer7/floatzel
mkdir lab0/grimer7/taillow
touch lab0/grimer7/weedle
touch lab0/grimer7/exploud
touch lab0/grimer7/marill
touch lab0/grimer7/squirtle
touch lab0/lillipup0
mkdir lab0/lumineon5
touch lab0/lumineon5/slugma
touch lab0/lumineon5/espeon
touch lab0/lumineon5/blitzle
mkdir lab0/lumineon5/weedle
touch lab0/omantype2
touch lab0/roggenrola9
echo  'Развитые способности No Guard' > lab0/drowzee3/karrablast
echo  'Способности\n Magical Leaf Storm' > lab0/drowzee3/bellossom
echo  'Способности Poison Sting String Shot\nBug Bite' > lab0/grimer7/weedle
echo  'Развитые способности Scrappy' > lab0/grimer7/exploud
echo  'Развитые\nспособности Sap Sipper' > lab0/grimer7/marill
echo  'Тип диеты\nHerbivore' > lab0/grimer7/squirtle
echo  'weigth=9.0 height=16.0 atk=6\ndef=5' > lab0/lillipup0
echo  'Возможности Overland=1 Jump=1 Power=2 Intelligence=3\nAmorphous=0 Egg Warner=0 Firestarter=0 Sinker=0' > lab0/lumineon5/slugmaecho  'Способности\nMing Mold Synchronize Trace' > lab0/lumineon5/espeon
echo  'Ходы Bounce Magnet Rise Signal\nBeam Sleep Talk Snore' > lab0/lumineon5/blitzle
echo  'Способности Constrict Withdraw Bite\nWater Gun Rollout Leer Mud Shot Brine Protect Ancientpower Tickle Rock\nBlast Shell Smash Hydro Pump' > lab0/omanyte2
echo  'weigth=39.7 height=16.0\natk=8 def=9' > lab0/roggenrola9

#2 task
chmod u=rwx,g=wx,o=rw  lab0/drowzee3
chmod 737 lab0/drowzee3/lickilicky
chmod 305 lab0/drowzee3/finneon
chmod 640 lab0/drowzee3/karrablast
chmod 400 lab0/drowzee3/bellossom
chmod 524 lab0/drowzee3/chimecho
chmod 500 lab0/drowzee3/venonat
chmod 330 lab0/grimer7
chmod 373 lab0/grimer7/floatzel
chmod 512 lab0/grimer7/taillow
chmod 444 lab0/grimer7/weedle
chmod 006 lab0/grimer7/exploud
chmod 644 lab0/grimer7/marill
chmod 004 lab0/grimer7/squirtle
chmod u=rw,g=w lab0/lillipup0
chmod 700 lab0/lumineon5
chmod g=r,o=rw lab0/lumineon5/slugma
chmod 622 lab0/lumineon5/espeon
chmod 644 lab0/lumineon5/blitzle
chmod 317 lab0/lumineon5/weedle
chmod 064 lab0/omanyte2
chmod g=rw,o=w lab0/roggenrola9

#3 task

chmod u+w lab0/drowzee3/bellossom
cat lab0/drowzee3/bellossom lab0/grimer7/marill > lab0/roggenrola9_73 #объединение в файл
chmod u-w lab0/drowzee3/bellossom


ln -s lab0/grimer7 lab0/Copy_57 #символическая ссылка

ln -s lab0/omantype2 lab0/lumineon5/slugmaomantype

ln lab0/lillipup0 lab0/grimer7/marilllillipup #жесткая ссылка

cat lab0/lillipup0 > lab0/drowzee3/karrablastlillipup

chmod u+r lab0/lumineon5/slugma
chmod u+rw lab0/lumineon5/weedle
cp -R lab0/lumineon5 lab0/lumineon5/weedle
chmod u-rw lab0/lumineon5/weedle
chmod u+r lab0/lumineon5/slugma

chmod u+w lab0/grimer7/taillow
chmod u+w lab0/omantype2
cp lab0/omantype2 lab0/grimer7/taillow
chmod u-w lab0/omantype2
chmod u-w lab0/grimer7/taillow

#4 task
wc -m lab0 >>/tmp/info 2> /tmp/trash | grep "^f"
ls -lRt 2> /tmp/trash | head -2
cat lab0/grimer7 2> /tmp/trash | grep -vi "e$"
ls -lRu lab0 2>&1 | grep "li"
cat -b lab0/roggenrola9 | grep -v "llo"
cat lab0/roggenrola9 2>&1 | grep -i "tk"

#5 task
chmod -R 777 lab0/omantype2
chmod -R 777 lab0/lumineon5/slugma
rm -r lab0/omantype2
rm lab0/lumineon5/slugma
rm lab0/lumineon5/slugmaomantype
rm lab0/grimer7/marilllillipup
chmod -R 777 lab0/grimer7
rm -R lab0/grimer7
chmod -R 777 lab0/lumineon5/weedle
rm -r lab0/lumineon5/weedle
