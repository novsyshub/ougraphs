## Formatting Guide
(I am going to preface this by saying I am notoriously bad at explaining things, so you have been warned.)
I figured it would probably be a good idea to summarize how my organization system works, since the compact clusters of nodes might be a bit confusing at first.
### Consecutive Operations
Nodes with outputs which are being passed directly from one to the other all in a row are layered with the first being at the bottom, and those following stacked on top. In case that's hard to imagine just from that description, here's a screenshot of one of those:
<picture>
    <source
        srcset="https://cdn.discordapp.com/attachments/1294386416314482721/1558963223015854130/image.png?ex=6acd5924&is=6acc07a4&hm=09b32907a01f51a419eae704fcace4615e8a3216df9cba38c0b6d99bd217367a"
        media="(orientation: portrait)" />
        <img src="https://cdn.discordapp.com/attachments/1294386416314482721/1558963223015854130/image.png?ex=6acd5924&is=6acc07a4&hm=09b32907a01f51a419eae704fcace4615e8a3216df9cba38c0b6d99bd217367a" alt = "" />
</picture>
---

### If/Else Statements
Like in the aforementioned example, the values passed to if/else statements are arranged from top to bottom in accordance to the location of their inputs:
<picture>
    <source
        srcset="https://cdn.discordapp.com/attachments/1294386416314482721/1558963955383271424/image.png?ex=6acd59d3&is=6acc0853&hm=640121bf265ea79863ecd04e0064eb9a8b9862417bee8b36abbe6a13a7d1909d" />
        <img src="https://cdn.discordapp.com/attachments/1294386416314482721/1558963955383271424/image.png?ex=6acd59d3&is=6acc0853&hm=640121bf265ea79863ecd04e0064eb9a8b9862417bee8b36abbe6a13a7d1909d" alt = "" />
</picture>
And since I know if/else confused the fuck out of me at first, have a shitty diagram I made in mspaint:
<picture>
    <source
        srcset="https://cdn.discordapp.com/attachments/909308566387707935/1558593238988890202/shitty_diagram.png?ex=6acd5211&is=6acc0091&hm=6b3463d3f8cdc99e2cb0c49b214196fc0cc646fabe41effd2c013b9d6cce7699" />
        <img src="https://cdn.discordapp.com/attachments/909308566387707935/1558593238988890202/shitty_diagram.png?ex=6acd5211&is=6acc0091&hm=6b3463d3f8cdc99e2cb0c49b214196fc0cc646fabe41effd2c013b9d6cce7699" alt = "" />
</picture>
---

### Final Outputs
Operations on an expression's input (initial value) and its output (final value) are clustered together, with the nodes arranged from front to back to indicate which operation happens first. Think of it as a "plus equals" or other equivalent.
Take this painfully bad example:
<picture>
    <source
        srcset="https://cdn.discordapp.com/attachments/1294386416314482721/1558958283572649984/vaguely_not_even_a_graph.png?ex=6acd548a&is=6acc030a&hm=64835ba0be19fa5fad9f04af55d4b3f7ecd063b7f344ee3bc390249d3896a69d"
        media="(orientation: portrait)" />
        <img src="https://cdn.discordapp.com/attachments/1294386416314482721/1558958283572649984/vaguely_not_even_a_graph.png?ex=6acd548a&is=6acc030a&hm=64835ba0be19fa5fad9f04af55d4b3f7ecd063b7f344ee3bc390249d3896a69d>" alt = "" />
</picture>
1. A (cyan) and B (magenta) are added together for a sum of C (red).
2. C is added to the original value of the tension flag (green), as defined by the default value and any changes done by the user for a sum of D (yellow).
3. D is passed on to the output node of tension, becoming the flag's new value.
---
Anyway that's about all I can think of right now :thumbsup:
Have fun