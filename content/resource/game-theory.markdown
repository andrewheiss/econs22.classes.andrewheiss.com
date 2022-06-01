---
title: Game theory
menu:
  resource:
    parent: Guides
type: docs
toc: true
weight: 2
---
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />
<script src="/rmarkdown-libs/kePrint/kePrint.js"></script>
<link href="/rmarkdown-libs/lightable/lightable.css" rel="stylesheet" />

<style type="text/css">
table {
  display: table;
}

.table td {
  vertical-align: middle;
  line-height: 1.1;
}
</style>



## Basic process for finding Nash equilibria

The easiest way to find Nash equilibria in a 2×2 game is to cover each column and row in turn and ask: "If player 1 knows that player 2 will choose X, what is player 1's best choice?" over and over again. Mark player 1's choice with a circle and mark player 2's choice with a dot. Any cells that have both a circle and a dot are equilibria.

Here's what that looks like in an invisible hand game. Anil and Bala need to choose what they're going to grow. Their payoffs (measured in utils) for each of their choices are listed in this matrix:

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

To start, cover up the column where Bala chooses to grow cassava. If Anil assumes that Bala chooses to grow rice, what's his best option? Anil would get 1 util from growing rice, and 4 from growing cassava. Cassava is best, so put a circle there.

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

Next, cover the column where Bala chooses to grow rice. If Anil assumes that Bala chooses to grow cassava, what's his best option? Anil would get 2 utils from growing rice, and 3 from growing cassava. Cassava is the best again, so put a circle there.

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

Regardless of what Bala chooses to do, Anil's best choice is always to grow cassava, so he'll do that. That's a pure, dominant strategy.

Let's go through the same process for Bala. Cover up the row where Anil chooses to grow cassava. If Bala assumes that Anil chooses to grow rice, what's his best option? Bala would get 3 utils from growing rice, and 2 from growing cassava. Rice is the best option, so put a dot there.

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> 🔵 <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

Next cover up the row where Anil chooses to grow rice If Bala assumes that Anil chooses to grow cassava, what's his best option? Bala would get 4 utils from growing rice, and only 1 from growing cassava. Rice is again his best option, so put a dot there.

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> 🔵 <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> ⭕ 🔵 <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

Bala's best option—regardless of what Anil chooses to do—is to grow rice, so that's what he'll do.

Phew. Finally we can look at it all together. Here's a summary of the different possible choices and responses:

- Best response for Anil if Bala chooses Rice = Cassava
- Best response for Anil if Bala chooses Cassava = Cassava
- Best response for Bala if Anil chooses Rice = Rice
- Best response for Bala if Anil chooses Cassava = Rice

There's a circle and a dot in the (4, 4) / (Cassava, Rice) square, which means that's the Nash equilibrium. That's the
situation that both players will naturally settle on without any outside communication, given the structure of the payoffs in the game.

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bala</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Rice </th>
   <th style="text-align:center;"> Cassava </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Anil</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Rice</span> </td>
   <td style="text-align:center;"> 🔵 <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">3</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Cassava</span> </td>
   <td style="text-align:center;"> ⭕ 🔵 <span style="color: #bf616a;">4</span> , <span style="color: #5e81ac;">4</span> </td>
   <td style="text-align:center;"> ⭕ <span style="color: #bf616a;">3</span> , <span style="color: #5e81ac;">1</span> </td>
  </tr>
</tbody>
</table>

## Mixed strategies

When there is no single Nash equilibrium in a game, players have to engage in a mixed strategy and attempt to predict what the other players will do. The choices they make are determined by the payoffs in the game, since it is generally more likely that players will choose strategies that maximize their payoffs. You need to calculate two things to do this:

1. Calculate the expected utility for each choice for each player and find the probability cutoff for each choice.
2. Calculate the expected payoff for each player.

These calculations involve actual math, unlike the more simpler approach of covering rows and columns and drawing circles and dots.

There are a bunch of helpful external resources and examples of how to do this, including these. You should check these out if you're interested in this game theory stuff:

- <i class="fas fa-external-link-square-alt"></i> [Policonomics, "Mixed strategies"](https://policonomics.com/mixed-strategy/)
- <i class="fas fa-external-link-square-alt"></i> [Game Theory 101, "Calculating payoffs of mixed strategy Nash equilibria"](http://gametheory101.com/courses/game-theory-101/calculating-payoffs-of-mixed-strategy-nash-equilibria/)
- <i class="fab fa-youtube"></i> [Game Theory 101, "Chicken"](https://www.youtube.com/watch?v=sww-Zsl0IRY) (a complete example of calculating everything in a chicken game)

Let's do this with the Bach or Stravinksy game that [we used in session 3](/content/03-content/):

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Friend 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Chinese </th>
   <th style="text-align:center;"> Italian </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Friend 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Chinese</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">1</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">0</span> , <span style="color: #5e81ac;">0</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Italian</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">0</span> , <span style="color: #5e81ac;">0</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
</tbody>
</table>

### Step 1: Find the equilibria

- Best response for Friend 1 if Friend 2 chooses Chinese = Chinese
- Best response for Friend 1 if Friend 2 chooses Italian = Italian
- Best response for Friend 2 if Friend 1 chooses Chinese = Chinese
- Best response for Friend 2 if Friend 1 chooses Italian = Italian

The game has two Nash equilibria, so it has a mixed strategy.

### Step 2: Calculate the expected utility for each choice for each player

We calculating the expected utility for each choice by assuming some probability for Friend 1's choices ($p$, `\(1 - p\)`) and for Friend 2's choices ($q$, `\(1 - q\)`):

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="3"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Friend 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:left;">    </th>
   <th style="text-align:left;">     </th>
   <th style="text-align:center;"> Chinese </th>
   <th style="text-align:center;"> Italian </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;"></span></span> </td>
   <td style="text-align:left;"> <span style=" font-weight: bold;    "></span> </td>
   <td style="text-align:left;">  </td>
   <td style="text-align:center;"> \(q\) </td>
   <td style="text-align:center;"> \(1 - q\) </td>
  </tr>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Friend 1</span></span> </td>
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Chinese</span> </td>
   <td style="text-align:left;"> \(p\) </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span> , <span style="color: #5e81ac;">1</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">0</span> , <span style="color: #5e81ac;">0</span> </td>
  </tr>
  <tr>
   
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Italian</span> </td>
   <td style="text-align:left;"> \(1 - p\) </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">0</span> , <span style="color: #5e81ac;">0</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">1</span> , <span style="color: #5e81ac;">2</span> </td>
  </tr>
</tbody>
</table>

To find the expected utility for a choice, add the utility × probability for each choice in the row (or column, for Player 2). Thus,

$$
`\begin{aligned}
EU_{\text{Friend 1, Chinese}} &= 2q + 0(1-q) =& 2q \\
EU_{\text{Friend 1, Italian}} &= 0q + 1(1-q) =& 1 - q \\
EU_{\text{Friend 2, Chinese}} &= 1p + 0(1-p) =& p \\
EU_{\text{Friend 2, Italian}} &= 0p + 2(1-p) =& 2 - 2p
\end{aligned}`
$$

With these formulas, you can then determine `\(q\)` and `\(p\)` by setting the expected utilities for each player equal to each other and solving for the variable:

$$
`\begin{aligned}
2q &= 1 - q & p &= 2 - 2p \\
3q &= 1 & 3p &= 2 \\
q &= \frac{1}{3} & p &= \frac{2}{3}
\end{aligned}`
$$

Friend 1's best response is determined by what Friend 2's `\(q\)` is in real life:

$$
\text{Best response}_{\text{Friend 1}} = 
\left \\\{ 
`\begin{aligned}
&\text{Chinese } & \text{if } q < \frac{1}{3} \\
&\text{Italian } & \text{if } q > \frac{1}{3} \\
&\text{indifferent } & \text{if } q = \frac{1}{3} \\
\end{aligned}`
\right \\\}
$$

Similarly, Friend 2's best response is determined by what Friend 1's `\(p\)` is in real life:

$$
\text{Best response}_{\text{Friend 2}} = 
\left \\\{ 
`\begin{aligned}
&\text{Chinese } & \text{if } p > \frac{2}{3} \\
&\text{Italian } & \text{if } p < \frac{2}{3} \\
&\text{indifferent } & \text{if } p = \frac{1}{3} \\
\end{aligned}`
\right \\\}
$$

### Step 3: Calculate the expected payoff for each player when playing the mixed strategy

The expected payoff is the utility × probability for each cell, added together. First, calculate the joint probabilities for each cell by multiplying the row and column probabilities:

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="3"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Friend 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:left;">    </th>
   <th style="text-align:left;">     </th>
   <th style="text-align:center;"> Chinese </th>
   <th style="text-align:center;"> Italian </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;"></span></span> </td>
   <td style="text-align:left;"> <span style=" font-weight: bold;    "></span> </td>
   <td style="text-align:left;">  </td>
   <td style="text-align:center;"> \(q = \frac{1}{3}\) </td>
   <td style="text-align:center;"> \(1 - q = \frac{2}{3}\) </td>
  </tr>
  <tr>
   <td style="text-align:center;vertical-align: middle !important;" rowspan="2"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Friend 1</span></span> </td>
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Chinese</span> </td>
   <td style="text-align:left;"> \(p = \frac{2}{3}\) </td>
   <td style="text-align:center;"> \(\frac{2}{3} \times \frac{1}{3} = \frac{2}{9}\) </td>
   <td style="text-align:center;"> \(\frac{2}{3} \times \frac{2}{3} = \frac{4}{9}\) </td>
  </tr>
  <tr>
   
   <td style="text-align:left;"> <span style=" font-weight: bold;    ">Italian</span> </td>
   <td style="text-align:left;"> \(1 - p = \frac{1}{3}\) </td>
   <td style="text-align:center;"> \(\frac{1}{3} \times \frac{1}{3} = \frac{1}{9}\) </td>
   <td style="text-align:center;"> \(\frac{1}{3} \times \frac{2}{3} = \frac{2}{9}\) </td>
  </tr>
</tbody>
</table>

Then multiply each probability by the payoff and add all the cells together:

$$
`\begin{aligned}
EP_{\text{Friend 1}} &= (2 \times \frac{2}{9}) + (0 \times \frac{4}{9}) + (0 \times \frac{1}{9}) + (1 \times \frac{2}{9}) =& \frac{2}{3} \\
EP_{\text{Friend 2}} &= (1 \times \frac{2}{9}) + (0 \times \frac{4}{9}) + (0 \times \frac{1}{9}) + (2 \times \frac{2}{9}) =& \frac{2}{3}
\end{aligned}`
$$

The expected payoff for each player in the mixed strategy is `\(\frac{2}{3}\)`, which is less than what either player would make if they coordinated on their least preferred outcome. That is, it's better for Friend 1 to compromise and eat Italian and get 1 unit of utility rather than gamble on the mixed strategy.
