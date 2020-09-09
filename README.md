comunicato stampa:
https://www.politicheagricole.it/flex/cm/pages/ServeBLOB.php/L/IT/IDPagina/15906

mappa google:
https://goo.gl/maps/zHq6JTpVxfM4bTpT8


excel regional alternativa
https://www.politicheagricole.it/flex/cm/pages/ServeBLOB.php/L/IT/IDPagina/11260


API per dettagli ....
https://docs.trefle.io/docs/guides/filtering
su valore singolo: https://trefle.io/api/v1/plants?token=mixdVlGen4ksQZvOSFDpQzIgtb8Ir_W3e0fmOd2olqI&filter[common_name]=beach%20strawberry


xls NAZIONALE:

ridotto decimali coord
rimosso non iscritti in elenco
aggiunto colonna note (filari o insiemi omogenei)


espansione tag tramite tabella wiki:
https://wiki.openstreetmap.org/wiki/Tag:natural%3Dtree/List_of_Genus,_Leaf_cycle,_Leaf_type
creato tabella tree_leaf 

alcuni genus potrebbero non essere sufficienti (Quercus è sia deciduous che evergreen, ma Quercus pubescens Willd. è solo deciduous
>> fatto a manina da openrefinea da finire (risolvi leaf_type TBD)

da talk-it: natural_monument:criteria=age;height; ecc




openrefine per natural_monument:criteria

if (cells["CR ETA"].value=="SI","age","")+
if (cells["CR CIRCONF"].value=="SI",";circumference","")+
ecc...

CR AMPIEZZA CHIOMA
crown?

CRITERIO FORMA O PORTAMENTO
shape?

CR VALORE ECOLOGICO
ecological_value?

RARITA' BOTANICA
rarity?

CRITERIO ARCHITETTURA VEGETALE
plant_architecture?
vegetal_structure?

CRITERIO VALORE PAESAGGISTICO
landscape


**** tipologia geometrica
messo tag note per non puntuali
resta da decidere altezza e criconferenza media e massima per gruppi/filari
