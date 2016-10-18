Antal brugere
-------------
2-6

Udviklingsmiljø
---------------
 * 1/4 kg mel
 * 2 æg
 * 1/4 øl
 * 1/2 l mælk
 * 1 spsk sukker
 * 1/2 tsk vanillesukker
 * lidt olie
 * lidt smør/margarine
 * pander


Program
-------

```Java
import skab.ingredienser;

Skål storSkål = new Skål();

storSkål.add(mel);
storSkål.add(æg);
storSkål.mix();
storSkål.add(mælk+øl);
storSkål.mix();
storSkål.add(sukker+vanillesukker);
storSkål.mix();
storSkål.add(olie);
storSkål.mix();

Pande p = new Pande();

while(!storSkål.tom()) {
  p.add(storSkål.getDej());
  p.steg();
  p.vend();
  p.steg();
  this.eat(p.getPandekage());
}
```

Sidenote
--------
Lav ALTID 8-dobbelt eller 16-dobbelt portion

Dette er en 8-dobbelt portion: ![Pandekage-stak](/images/ohms-pancakes.jpg)
