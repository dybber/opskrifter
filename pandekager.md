<link id="linkstyle" rel="stylesheet" href="foghorn.css">
<meta http-equiv="Content-Type" content="text/html;charset=UTF-8">


Antal brugere
-------------
4-12

Udviklingsmiljø
---------------
 * 1/2 kg mel
 * 4 æg
 * 1/2 øl
 * 1 l mælk
 * 2 spsk sukker
 * 1 tsk vanillesukker
 * lidt olie __gange 2__
 * lidt smør/margarine __gange 2__
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
