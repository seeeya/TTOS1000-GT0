# Versionhallintahaara (Branch)

Kuvauksen kirjoitti: Rami Ojala, K8412

## Lyhyt kuvaus

Versionhallinnassa, Haara, eli Branch on Masterin kopio, johon ollaan vapaita tekemään muutoksia vaikuttamatta Masterin haaraan. Brancheja käytetään, jotta voidaan koodata useita ominaisuuksia samanaikaisesti (tai debugata ja korjata useita virheitä samanaikaisesti). Yksinkertaisessa Git Workflow:ssa haaraudutaan suoraan Masterista kun aletaan tehdä uutta ominaisuutta, kun ominaisuus on valmis, pullataan Masteri vielä uudestaan siltä varalta, että Masteriin on tullut muutoksia, sitten testataan että mikään ei mennyt rikki ja pusketaan ominaisuus haara takaisin Masteriin.

## Esimerkkejä

Master Branch, sisältää testatun ja toimivaksi todetun koodin. Joissain Git Workflow:ssa tästä haarasta, haaraudutaan Release 1.0, 1.1, ... n, 2.0 haaroihin.

Test Branch, Tämä haara sisältää koodin, joka on valmiina Hyväksyntä testaukseen. Hyväksyntä testauksen läpäistyä tämä mergetään masterrin.

Development Branch, Tämä haara sisältää testaamattoman valmiin koodin.

Feature Branch, Tämä haara vedetään Development Branchista, kun aletaan tekemään uutta ominaisuutta ohjelmistoon ja haaran elinkaaren lopussa Mergetään takaisin development branchiin odottamaan testausta.

Issue (Hotfix) Branch, Tämä haara, riippuen Workflow:sta vedetään Master Branchista ja korjauksen löydyttyä pusketaan, sekä Master branchiin, että Development branchiin

## Lähteitä liittyen aiheeseen

Mitä lähteitä löysit liittyen annettuun aiheeseen/käsitteeseen?

* [Git Branching and Merging Strategies (24:16))](https://www.youtube.com/watch?v=to6tIdy5rNc)
* [Atlassian Stash - Git workflows in the Enterprise (36:05))](https://youtu.be/gLWSJXBbJuE)
* [Wikipedia linkki Branchista](https://en.wikipedia.org/wiki/Branching_(version_control))

## Linkit wikin muihin sivuihin

Kerää tähän sivut wikin sisältä, jotka mielestäsi liittyvät kuvaamaasi käsitteeseen/aiheeseen

* [Etsi tähän linkki toiseen wikin sisällä olevaan sivuun, joka liittyy oleellisesti omaan aiheeseesi]()
