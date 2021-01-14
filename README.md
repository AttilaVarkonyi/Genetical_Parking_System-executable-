# Genetical_Parking_System-executable-
# Genetical_Parking_System
# Felhasználói dokumentáció
A felhasználói dokumentáció lényege, hogy leírást adjunk a kész játék futtatásának módjáról, továbbá, hogy a felhasználó tisztában legyen a legfontosabb tudnivalókkal a szoftverrel kapcsolatban, illetve a játék felülettel.
## Telepítés
Szoftverünk nem igényel telepítést, egyszerűen kattintsunk a GeneticalParkingSystem.exe fájlra, és a játék elindul. A futtatható állomány természetesen a dolgozathoz mellékelt lemezen elérhetők lesznek.
 
RENDSZERKÖVETELMÉNYEK
Operációs rendszer:	Windows 7, Windows 10
CPU:	x86, x64
Grafikus API:	DX10, DX11 vagy DX12 kompatibilis
Tárhely:	60 MB

Futtatáskor a játék elindul, a genetikus algoritmus rögtön elkezd működni, és az ágens első generációja pedig már keresik az utat a kijelölt parkolóhelyre. Az ezt követő generáció ez előbbi eredményeitől vezérelve már nagyobb eséllyel közelíti meg a cél-parkolóhelyet, és így tovább egészen addig, amíg az első kocsi nem áll be sikeresen.
A felület bal felső sarkában található egy „Exit” gomb, amivel az alkalmazás bezárható, továbbá a képernyő bal alsó sarkában olvashatunk adatokat a genetikus algoritmus működésével kapcsolatban, azaz, hogy hányadik generációnál járunk, hány tagból áll egy generáció, hány százalék a mutációs ráta, mi az átlag fitness, illetve a legjobb egyed fitness száma.
Elindításkor az első generáció a parkoló elején megjelenve elkezd szabadon cirkálni.
 
A genom kezdeti random kialakításától függ, hogy az ágens mennyi idő alatt, hány generációváltás után talál be a parkolóba. Ez szerencsés kiosztás esetén megtörténhet már a negyedik generáció végén, de inkább jellemzőbb a 20. és a 30. generáció között. Rosszabb esetben pedig a kívánt eredmény még többet várathat magára. Amint egy ágens sikeresen beáll a kívánt parkolóba, úgy az összes kocsi leáll, és megáll a szaporodási ciklus.
