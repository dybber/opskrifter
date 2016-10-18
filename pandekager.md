<link id="linkstyle" rel="stylesheet" href="foghorn.css">
<meta http-equiv="Content-Type" content="text/html;charset=UTF-8">


Antal brugere
-------------
1-3

Udviklingsmiljø
---------------
 * 1/8 kg mel
 * 1 æg
 * 1/8 øl
 * 1/4 l mælk
 * 1/2 spsk sukker
 * 1/4 tsk vanillesukker
 * lidt olie
 * lidt smør/margarine


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
