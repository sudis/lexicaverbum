# Numbers Game Tutorial
**Numbers** is similar to a __roulette gamble__ in its simplest terms, but there are also aspects where it differs. As in roulette, you can place bets on **groups of numbers**. Unlike roulette, here the **smallest set** of numbers brings the biggest win. The earnings table of all groups is given below.
```fix
Number Group | Earning Multiplier
---------------------------------
100          | x10.0 [MAX WIN]
99 - 90      | x2.0
89 - 80      | x2.2
79 - 70      | x2.4
69 - 60      | x2.6
59 - 51      | x2.8
50           | x10.0 [MAX WIN]
49 - 40      | x3.0
39 - 30      | x3.2
29 - 20      | x3.4
19 - 10      | x3.6
9 - 2        | x3.8
1            | x10.0 [MAX WIN]
```
We said it was different from roulette, right? Numbers is actually a game that needs to be **played twice** in one go. Let's show an example usage command to explain this better.

`/numbers play [bet: 1000] [group: 59-51] [choice: increase OR decrease]`

In the **first** part, we determine how much we should bet. In the **second part**, we indicate the group that we think will win. In the **last part, you choose whether to increase or decrease**. As we just said, we said that **Numbers is a game played twice in a row**. The number in the first game is **kept in memory** and when the second game is played, it is *__**combined**__* with the result in the first game to form a new group.

Let the number `35` be obtained in the first game. In the second game, let our lucky number be `13`. He would win the group `19 - 10` in the second game, right? **No**, `13` is added to the number of `35` that appeared in the first game. So our lucky number would be `48`. Therefore, our lucky group rises to the `49 - 40` group. If we had chosen "**decrease**" in the last part, then we would have subtracted from this number rather than added.

`❗` Remember, that our lucky numbers range from **1** to **100**. Therefore, in the second part, if you **exceed** 100 or 1 during addition or subtraction, you are automatically **defeated**.
