# Aufgabe 3
(Aus dem "Advent of Code" 2021, Im englischen Orginal hier: https://adventofcode.com/2021/day/1)

Gegeben ist eine Liste von Zahlen.

Beispielzaheln: 199, 200, 208, 210, 200, 207, 240, 269, 260, 263

Echter Input: https://github.com/mariusleckebusch/Aufgabe-3/blob/master/input.txt

Frage: Wieviel Elemente in der Liste sind größer als der direkte Vorgänger?

Antwort: Es sind 1752 Elemente größer als der direkte Vorgänger

Code:
```js
var input = [
// https://github.com/mariusleckebusch/Aufgabe-3/blob/master/input.txt
]

var increased = [];
var decreased = [];


for(var i = 0; i < input.length; i++) {
    var previousItem = input[i-1];
    var Item = input[i];
    if(previousItem < Item) {
        console.log(Item + " (increased)")
        increased.push(i)
    } else {
        console.log(Item + " (decreased)")
        decreased.push(i) 
    }
        
}

console.log(increased.length)
console.log(decreased.length)
```
