# LeekWars

LeekWars est un site Internet dans lequel il est possible de faire combattre des poireaux (oui oui, des poireaux) entre eux. Le but est de faire progresser ses poireaux en les faisant combattre contre d'autres poireaux, et ainsi devenir le meilleur poireau de tous les temps.

Dans LeekWars, il n'existe pas de contrôles. Le joueur ne joue pas, il programme son poireau pour que celui-ci soit complètement autonome.

Faisons nos premiers pas dans l'intelligence artificielle ensemble à l'aide de LeekWars !

> 🚀 Cette activité est encadrée par le Coding Club d'Epitech.\
> ❓ Si vous avez des questions ou que vous bloquez sur l'une des étapes, vous pouvez demander de l'aide aux autres participants autour de vous (l'entraide est primordiale à Epitech 😄).\
> S'ils ne parviennent pas à vous débloquer, n'hésitez pas à appeler un *Cobra*, identifiables à l'aide de leurs super polos ⭐

## Etape 0 : Créons notre premier poireau

Rendez-vous sur le site de [LeekWars](https://leekwars.com/).

Vous devriez arriver sur une page qui ressemble à celle-ci :

![Page d'accueil](./assets/landing.png)

> 💡 Vous pouvez mettre LeekWars en français en cliquant sur le drapeau.

Cliquez sur le bouton "S'inscrire" (ou `Sign Up`) en haut à droite de la page.

Renseignez ensuite le nom de votre poireau, et ajoutez des éléments de personnalisation à votre guise. Vous pouvez par exemple changer la couleur des feuilles de votre poireau et lui ajouter un chapeau 🎩

## Etape 1 : Jettons un oeil à l'interface

Nous voici désormais sur un magnifique interface ! Voyons voir ce qu'on a là...

![Interface](./assets/interface.png)

En haut à droite de l'écran, nous avons diverses informations utiles.

- En premier lieu, nous voyons notre monnaie : cette ressource sera très utile pour améliorer son poireau par la suite ! Elle s'acquiert en gagnant des combats.
- A coté de la monnaie, nous voyons notre rang. Il s'agit d'un score qui augmente à chaque fois que votre poireau gagne un combat, et qui diminue à chaque fois qu'il en perd un. Plus votre rang est élevé, plus vous affronterez des adversaires coriaces. 

> :bulb: Cela s'apparente à un système de `MMR` ! Vous pouvez en apprendre plus [ici](https://hitmarker.net/what-does-mmr-mean#:~:text=Matchmaking%20Rating%2C%20or%20'MMR',and%20achieved%20a%20minimum%20MMR).

- Les deux icônes à droite sont la boite aux lettres et les notifications, et l'icone à gauche permet d'accéder aux paramètres.
- Enfin, le bouton `Profil` permet d'accéder à votre page de profil, où vous pouvez ajouter différentes informations sur vous-même.

### Passons au centre de l'écran !

Au centre de l'écran, nous pouvons retrouver une synthèse de notre poireau et de nos statistiques, mais nous pouvons également les améliorer !

Nous voyons également notre inventaire : nous possédons actuellement une arme, notre bon vieux `pistolet` ! :gun:

Enfin, à gauche de l'écran, il existe différents boutons : `Editeur`, `Potager` et `Marché` sont les plus importants et sont ceux dans lesquels vous passerez le plus de temps :slight_smile:

> 💡 Nous vous conseillons de visiter les différentes pages du jeu pour vous familiariser avec l'interface. Vous y découvrirez peut-être déjà quelques fonctionnalités de LeekWars que nous n'avons pas encore expliqué...

⚠️ Nous sommes brièvement passés sur le système de statistiques sans plus de détails.

Pour faire court, votre poireau possède un niveau (il commence au niveau 1), et chaque montée de niveau lui donne un **point de capital**. Vous pouvez investir chaque point de capital dans une statistique, permettant d'augmenter différentes stats telles que sa vie, sa puissance, sa vitesse mais encore différents aspects "programmatiques" tels que la quantité de mémoire et la puissance du processeur qui exécutera votre code en combat !

> 🚀 Vous disposez de 50 points de capital. Vous pouvez les investir dès maintenant, mais nous vous recommandons de continuer à découvrir le jeu avant de les utiliser, afin de savoir quelles statistiques vous souhaitez améliorer en priorité.

Assez lu ? Ca tombe bien, tous dans le ring maintenant !

## Etape 2 : Lançons nos premiers combats

Passons sans plus tarder aux combats, ce pourquoi nous sommes tous ici (et la programmation aussi, évidemment. Mais surtout les combats) :crossed_swords:

Rendez vous dans la section `Potager`. Vous devriez voir apparaitre votre poireau, ainsi que d'autres poireaux en dessous de celui-ci. Ce sont vos adversaires ! Cliquez sur n'importe lequel d'entre eux pour lancer un combat !

Une fenêtre s'ouvre alors. Vous pouvez observer le combat entre vous et votre adversaire.

![Combat](./assets/combat.png)

> :bulb: Vous avez accès à différentes informations sur cet écran, en plus de voir le combat. Cela pourra vous être très utile lorsque vous commencerez à améliorer le programme de votre poireau !

Tour à tour, nous voyons les actions de notre poireau et de celui de notre ennemi s'effectuer : on voit qu'ils se rapprochent jusqu'à être à une distance assez proche, puis s'échangent des coups jusqu'à ce que mort s'en suive.

Vous avez gagné ? Félicitations ! :trophy: \
Vous avez perdu ? Dommage... :cry:

Ce que ce combat vous a surtout appris, c'est une nouvelle notion du jeu : le mouvement et les actions.

> :bulb: De base, votre poireau possède 3 points de mouvement et 10 points d'action. \
> Cela signifie qu'il peut se déplacer de 3 cases par tour, et effectuer des actions valant un total de 10 points maximum. Chaque action possède son nombre de points requis !

Il est très important d'**observer** le comportement de votre poireau : cela vous aidera à comprendre son comportement. 

Lorsqu'une situation ne se passe pas comme prévu, vous pourrez vous baser sur ce que vous avez vu pour essayer de déterminer le problème (indice : il viendra très certainement de votre code :thinking:)

En plus de l'évolution de votre rang, votre combat vous octroie différentes récompenses, et ce même si vous perdez. Ne vous inquiétez pas, ce premier combat vous est bénéfique même si vous ne l'avez pas gagné. :wink:

Jetons un oeil à l'interface suivant :

![Summary](./assets/summary.png)

J'ai perdu :cry: mais cela ne m'a pas empêhé de gagner des Habs, la monnaie dont on parlait tout à l'heure ! :dollar:

En revanche, mon poireau n'a pas gagné beaucoup d'expérience. Il faudra gagner le combat pour cela !

> :trophy: J'ai également gagné des trophées. Ces derniers sont des succès que vous pouvez gagner en accomplissant différentes actions dans le jeu. \
> Leur utilité principale ? Aucune, si ce n'est le **flex** bien sûr !

Nous pourrions nous amuser à lancer des combats en boucle de la sorte, jusqu'à ce que notre poireau finisse par gagner ou monter de niveau. Mais on ne vous conseille pas de faire cela sans toucher au **programme** de votre poireau, et ce pour deux raisons :

- Même si vous gagnez les premiers combats, vous allez vite vous mesurer à des poireaux dont les programmes ont été modifiés. Et n'oubliez pas : le premier challenge est de réussir à contrer la stratégie de base de votre poireau, c'est donc ce sur quoi seront spécialisés vos adversaires ! Coriace...
- Vous n'avez droit qu'à **100 combats**. Cette limite se régénère avec le temps (ou en achetant avec vos *Habs*), mais ce seront peut-être vos seuls combats de la journée, ce serait dommage de les gaspiller !

Apprenons à triompher de nos ennemis avant de retourner dans le potager. Et pour cela, rentrons dans le vif du sujet : la **programmation** ! :heart:

## Etape 3 : Modifions le programme de notre poireau

TODO: Donner une première piste d'amélioration en guidant vers une première solution

Expliquer les concepts basiques de la programmation (variables, conditions, boucles...) en rappelant que les Cobra sont là pour aider

## Etape 4 : Montée de niveau rime avec nouveaux pouvoirs !

TODO: Expliquer les différents items du market et leur pertinence: armes avec différentes range/damage/fire, potions avec différents effets et chips

Expliquer leur intégration dans le code

## Etape 5 : Améliorons notre IA

TODO: Farmer les combats pour acquérir plus de niveau

Expliquer différentes stratégies possibles (distance, tank, heal, etc.)

## Etape 6 : L'étape 6

Félicitations, vous avez désormais toutes les bases nécessaires pour jouer à LeekWars !

Le plus important pour vous à partir de maintenant sera d'avoir un poireau qui saura faire face à tout type de situation loufoque et d'agir en conséquence.

N'oubliez pas : plus vous combattrez, plus vous monterez en rang, et plus vous affronterez des adversaires coriaces. Ajustez votre stratégie en permanence pour triompher de vos ennemis !

> Désormais, la [documentation](https://leekwars.com/help/documentation) devient votre meilleure amie 😉

## Et si on faisait un tournoi ? 🏆

Quoi de mieux qu'un petit tournoi pour vous départager et élire le meilleur éleveur de poireau de ce Coding Club 🔥

Regroupez-vous avec les personnes proches de vous pour créer une équipe (une personne peut le faire sur son profil, puis les autres peuvent la rejoindre en cliquant sur un lien similaire à celui-ci: [https://leekwars.com/team/8740](https://leekwars.com/team/8740), en remplacant l'ID par celui de votre équipe).

Désormais, attendez qu'un Cobra prépare la liste des équipes qui s'affronteront dans le tournoi 😄

> Vous pouvez peaufiner votre statégie pour prendre en compte les combats d'équipe, qui ont une particularité : chaque équipe possède une tourelle sur le champ de bataille.

> Attention, celle-ci a beaucoup de points de vie, mais si vous arrivez à la détruire, vous gagnez. 🎖️\
> Vous pouvez également gagner en tuant tous les poireaux adverses, comme sur les combats individuels.
