# js1k-2023

JS1K 2023 - Lucky the Rad Dragon

## playtest notes

### bugs

I think level is off by one, you should only be able to get up to 5, and should
match the costs of the weapons and shields - maybe start player at 0 for ease?

### balance

enemies don't scale well, they're too easy, they never have challenging atk
(though I did max build my player - try with weaker builds)
you level up way faster than you get money to buy weapons and shields
you do too much damage - just use 2 + pweapon + ( plevel - 1 ) maybe

## minifying 

main has no golfing applied

nb - we can get about 56 bytes when we remove let and const etc, so assume
that we are good around 1080 bytes or so

let's start making branches

the goal is:

2175B 
1966B from branch no-more-lines, merged into main
1932B from minor in main (should have been done in no-more-lines)
-1955B from branch cat-adjacent-appends, worse, did not merge into main
1919B from branch button-helper-fn
1894B from branch inline-temps
1880B from branch inline-temps revision
1664B from branch brutal-display-rip
1654B from minor in main
1798B from branch no-state, worse, did not merge into main
