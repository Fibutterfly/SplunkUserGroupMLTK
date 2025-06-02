
Ez csak szemléltetés.  
![hiányzó értékek](../presentation/103_01_missingvalue.png)  
A null értékek mindig bezavarnak, mert nem számok, így nem tudunk rajtuk értelmesen matematikai műveletek végezni. Ehhez viszonylag sok bevált módszer van, a teljesség igénye nélkül:
- konstans
- előző érték
- következő érték
- valamilyen középérték valamilyen ablak segítségével
- interpolációs technikák, mint spline, lineáris.

Ezeket a feladatnak megfelelően érdemes megválasztani. Jelen esetben a mostani és a következő mérés közötti mértani átlagot választom.  
![Becslés](103_02_fillmissingvalue.png)

Az ábráján pedig már remekül látszódik a napon belüli ciklikusság (cikk-cakk) és a napokon túl mutató ciklikussák (oszcilláció).  
![gráf](../presentation/103_03_cylic.png)  