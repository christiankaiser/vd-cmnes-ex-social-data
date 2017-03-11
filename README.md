# Exemple de données socio-démographiques pour les communes du canton de Vaud

Ce répértoire contient à la fois quelques données statistiques ainsi que les géométries des communes, à l'état de 2015.

Les fichiers `cmnes_vd_data.tsv` est `cmnes_vd_data.xlsx` contiennent une série de 15 indicateurs statistiques sur les 318 communes vaudoises, extraites depuis l'[atlas statistique de Statistique Vaud](http://www.scris.vd.ch/Default.aspx?DomId=2091).

Le fichier Shape `vec200_cmnes_vd_2015` contient les limites communales des mêmes 318 communes vaudoises. Il s'agit d'un extrait des limites communales 2015 de la carte du [Vector200 de Swisstopo](http://www.swisstopo.admin.ch/internet/swisstopo/fr/home/products/landscape/vector200.html). Le fichier original est disponible sur [https://github.com/interactivethings/swiss-maps/](https://github.com/interactivethings/swiss-maps). Le système de référence spatial du fichier est CH1903/LV03 (EPSG:21781), et l'encodage du fichier DBF est en ISO-8859-1.

Les copyrights sont décrits sur les sites respectifs.


Le fichier Shape `vec200_cmnes_vd_2015_pts` contient un point par commune, situé à l'intérieur du polygone de la commune. Ces points ne correspondent pas au centroïde car un centroïde peut potentiellement se situer à l'extérieur du polygone (comme p.ex. à Lausanne). Les points ont été générés à l'aide de la fonction `ST_PointOnSurface` de PostGIS, puis édités pour un placement optimal.
