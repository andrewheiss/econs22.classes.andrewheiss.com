---
title: "Problem set 2"
linktitle: "Problem set 2"
date: "2022-06-20"
due_date: "2022-06-20"
due_time: "11:59 PM"
menu:
  assignment:
    parent: Problem sets
    weight: 2
type: docs
toc: true
weight: 2
editor_options: 
  chunk_output_type: console
---
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




**Submit this as a PDF on iCollege.** You can use whatever you want to make your drawings, including [Gravit Designer](https://gravit.io/), Adobe Illustrator, Excel, PowerPoint, Microsoft Paint, or photographed/scanned pen and paper.

**Cite your sources and show your work.**


## 1

The following game represents the interaction between two software engineers, Astrid and Bettina, who are working together to write code as a part of a project. Astrid is better at writing Java code, while Bettina prefers C++. The numbers represent the pay in dollars for completion of the project. 

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Bettina</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Java </th>
   <th style="text-align:center;"> C++ </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Astrid</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Java</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">$4,000</span>???,???<span style="color: #5e81ac;">$3,000</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">$2,000</span>???,???<span style="color: #5e81ac;">$2,000</span> </td>
  </tr>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Astrid</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">C++</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">$0</span>???,???<span style="color: #5e81ac;">$0</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">$3,000</span>???,???<span style="color: #5e81ac;">$6,000</span> </td>
  </tr>
</tbody>
</table>

&nbsp;

Based on this information, which of the following are true? Why or why not? **Explain why or why not in a sentence for each.**

1. There are two Nash equilibria: (Java, Java) and (C++, C++).

1. If Astrid can choose the language first and commit to it, then (Java, Java) will be chosen.

1. If the two can make an agreement beforehand, including a transfer of $500 from Bettina to Astrid, then (C++, C++) will be chosen.

1. If the two can make an agreement beforehand, including a transfer of $2,000 from Bettina to Astrid, then (C++, C++) will be chosen.

1. If the two cannot make an agreement beforehand, then they may end up with the (Java, C++) outcome.


## 2

Consider a repeated prisoners' dilemma game with a finite number of rounds.

1. If we assume that all parties are narrowly rational, and that they know which is the last period, why would we predict no cooperation during the whole game? **Answer in a sentence.**

1. Why, in practice, might parties not behave this way? **Answer in ???30 words.**

In the prisoners' dilemma computer tournament described in the Radiolab episode, the *Tit for Tat* strategy won. This was also the case in the ["Evolution of Trust"](http://ncase.me/trust/) game that you played.

3. In what sense, exactly, did it win? **Answer in a sentence.**

1. How robust was this finding? Are there situations where *Tit for Tat* is too nice? Too provocable? Too forgiving? **Answer in ???30 words.**


## 3

The inherent negativeness in political campaigns is often described as a classic prisoner's dilemma. 

1. Write down a payoff matrix that shows the choice between positive and negative campaigning as a prisoner's dilemma.

1. Give a recent real-life example of a negative campaign prisoner's dilemma. **Answer in ???30 words.**

In class, I argued that negative political campaigning might be better modeled as a stag hunt.

3. Why did I say this? What is the difference between a stag hunt and a prisoner's dilemma? **Answer in ???50 words.**

1. Write down a payoff matrix that shows the choice between positive and negative campaigning as a stag hunt.


## 4

After Hurricane Maria, hundreds of nonprofit organizations streamed to Puerto Rico and other Caribbean islands to provide disaster relief. [Research has found](https://theconversation.com/response-to-natural-disasters-like-harvey-could-be-helped-with-game-theory-83125) that coordination between nonprofits during disasters is difficult to maintain???it's easy for individual nonprofits to fundraise and pursue programming on their own while ignoring other organizations working on the same issues. Additionally, there are incentives to do projects that are cheap and have fast turnaround, since [donors respond to the visibility of organizations providing disaster relief](https://www.sciencedirect.com/science/article/pii/S092552730900365X).

Consider two nonprofit organizations working in Puerto Rico. Together, they could spend time coordinating their efforts and run a shelter for hurricane victims, providing each organization with 100 utils. Alternatively, they could individually distribute paper towels???a simple, low-cost, fast, and [visible](https://www.cnn.com/videos/politics/2017/10/03/donald-trump-puerto-rico-supplies-von.cnn/video/playlists/trumps-response-to-puerto-rico-crisis/) project???and receive 5 utils. 

This situation can be modeled with the following payoff matrix:

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Nonprofit 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> Run shelter </th>
   <th style="text-align:center;"> Distribute paper towels </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Nonprofit 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Run<br>shelter</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">100</span>???,???<span style="color: #5e81ac;">100</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">0</span>???,???<span style="color: #5e81ac;">5</span> </td>
  </tr>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Nonprofit 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">Distribute<br>paper<br>towels</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">5</span>???,???<span style="color: #5e81ac;">0</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">5</span>???,???<span style="color: #5e81ac;">5</span> </td>
  </tr>
</tbody>
</table>


1. What are the consequences of this kind of interaction? What will the two organizations naturally tend to do? Why? (i.e. what are the equilibria?) **Answer in ???30 words.**

1. What kind of game is this? Why? Can cooperation be ensured? How? **Answer in ???20 words.**

1. **Extra credit:** In the absence of communication, what are the two nonprofits' mixed strategies? (See [the guide in the resources section](/resource/game-theory/) for how to calculate mixed strategies.) How will they guess what the other organization will do? Under what conditions will nonprofit 1 choose to run the shelter? (i.e. what are the probability cutoffs for each nonprofit choosing to run the shelter or distribute paper towels?) **Answer in ???40 words. Show your work.**

1. **Extra credit:** What is the expected payoff of engaging in a mixed strategy? (i.e. choosing to gamble based on probability cutoffs rather than communicate and coordinate in person?) **Show your work.**


## 5

[A recent poll by the Edelman Trust Barometer](https://www.edelman.com/trust-barometer) shows a staggering drop in trust in private and public institutions in the United States. Only 33% of Americans surveyed have trust in government, and "no country saw steeper declines than the United States, with a 37-point aggregate drop in trust across all institutions"

1. Why does a community with a high level of trust have an advantage over one with lower levels of trust? (*Hint*: recall your reading from Mayer, 2014 on stag hunts) **Answer in ???40 words.**

1. To what extent can the institution of trust be thought of as a cooperative equilibrium in a stag hunt game? **Answer in ???30 words.**

1. How might a cooperative equilibrium degenerate into a non-cooperative equilibrium? **Answer in ???30 words.**


## 6

Consider **the society you live in,** or **another society** with which you are familiar.

1. To make society fairer (according to the substantive judgment of fairness), would you want greater equality of income, happiness, or freedom? Why? Would there be a trade-off between these aspects? (**???30 words**)
1. Are there other things that should be more equal to achieve greater substantive fairness in this society? (**???30 words**)
1. How fair is this society, according to the procedural judgment of fairness? (**???30 words**)
1. Suppose that, behind a Rawlsian veil of ignorance, you could choose to live in a society in which one (but only one) of the three procedural standards for fairness (voluntary exchange of property, equality of opportunity, and deservingness) would be the guiding principle for how institutions are organized. Which procedural standard would you choose, and why? (**???50 words**)


## 7

1. Two farmers have unlimited access to a common plot of land and can let their cows graze on it. The matrix below shows the benefits they get from grazing either 1 or 2+ cows on the land.

    1. What category of game is this?
    2. What is/are the Nash equilibrium/equilibria?
    3. What is/are the Pareto efficient outcome(s) in this game?

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Farmer 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> 1 cow </th>
   <th style="text-align:center;"> 2+ cows </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Farmer 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">1<br>cow</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">8</span>???,???<span style="color: #5e81ac;">8</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span>???,???<span style="color: #5e81ac;">10</span> </td>
  </tr>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Farmer 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">2+<br>cows</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">10</span>???,???<span style="color: #5e81ac;">2</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">4</span>???,???<span style="color: #5e81ac;">4</span> </td>
  </tr>
</tbody>
</table>

2. The government offers a reward or subsidy for communities where farmers only allow 1 cow to graze on the common field, resulting in a new payoff matrix.

    1. What category of game is this?
    2. What is/are the Nash equilibrium/equilibria?
    3. What is/are the Pareto efficient outcome(s) in this game?

<table class="table" style="width: auto !important; margin-left: auto; margin-right: auto;">
 <thead>
<tr>
<th style="empty-cells: hide;border-bottom:hidden;" colspan="2"></th>
<th style="border-bottom:hidden;padding-bottom:0; padding-left:3px;padding-right:3px;text-align: center; " colspan="2"><div style="border-bottom: 1px solid #ddd; padding-bottom: 5px; "><span style="color: #5e81ac;">Farmer 2</span></div></th>
</tr>
  <tr>
   <th style="text-align:center;">   </th>
   <th style="text-align:center;">    </th>
   <th style="text-align:center;"> 1 cow </th>
   <th style="text-align:center;"> 2+ cows </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Farmer 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">1<br>cow</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">15</span>???,???<span style="color: #5e81ac;">15</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">2</span>???,???<span style="color: #5e81ac;">10</span> </td>
  </tr>
  <tr>
   <td style="text-align:center;"> <span style="-webkit-transform: rotate(270deg); -moz-transform: rotate(270deg); -ms-transform: rotate(270deg); -o-transform: rotate(270deg); transform: rotate(270deg); display: inline-block; "><span style=" font-weight: bold;    color: #bf616a !important;">Farmer 1</span></span> </td>
   <td style="text-align:center;"> <span style=" font-weight: bold;    ">2+<br>cows</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">10</span>???,???<span style="color: #5e81ac;">2</span> </td>
   <td style="text-align:center;"> <span style="color: #bf616a;">4</span>???,???<span style="color: #5e81ac;">4</span> </td>
  </tr>
</tbody>
</table>

3. How is Pareto efficiency different from fairness? (**???30 words**)
