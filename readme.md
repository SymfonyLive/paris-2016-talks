# [Symfony Live - Paris 2016](http://paris2016.live.symfony.com/) talks

- All talks are in **french**.
- Comment and rate talks on [joind.in](https://joind.in/event/symfonylive-paris-2016)

## Monolith Repositories with Git

<dl>
  <dt>Description</dt>
  <dd>Google and Facebook store their codebase into one giant code repository. Symfony has been doing the same thanks to Git and some secret sauce with great success since 2010. Having only one repository makes code management much easier for end users and core contributors: one central place to submit pull requests and report bugs, simple cross-project atomic changes, fast releases, and more. But what about users wanting to use only one component? Enter "repository splitting". After learning some theory about subtree splits and how to create them with the Git built-in but slow "subtree" command, I will talk about the tool I developed using libgit2 and Go to make the process almost real time. If you have a microservice oriented architecture and manage one repository per microservice, you could probably benefit from using the same technique with one repository for development and read-only splits for packaging and deployment.</dd>
</dl>

~~Slides~~  
~~Video~~

By [Fabien Potencier](https://connect.sensiolabs.com/profile/fabpot)  
![github](icon/github.png) [@fabpot](https://github.com/fabpot)  
![twitter](icon/twitter.png) [@fabpot](https://twitter.com/fabpot)

---

## Guard dans la vraie vie

<dl>
  <dt>Description</dt>
  <dd>Le nouveau component Guard simplifie la mise en place d'authentification sur nos applications Symfony. Avec une classe par système d'authentification, voyons comment personnaliser les différentes étapes et comment ajouter facilement de nouveaux Guard authenticator à son application Symfony.</dd>
</dl>

~~Slides~~  
~~Video~~

By [Jérémy Romey](https://connect.sensiolabs.com/profile/jeremyfreeagent)  
![github](icon/github.png) [@jeremyFreeAgent](https://github.com/jeremyfreeagent)  
![twitter](icon/twitter.png) [@jeremyFreeAgent](https://twitter.com/jeremyfreeagent)

---

## R2D2 to BB8

<dl>
  <dt>Description</dt>
  <dd>La migration continue d'un vieux projet n’est pas une mince affaire. En premier lieu, il faut définir un périmètre minimal de fonctionnalités à transférer de l'ancien projet au nouveau, et mettre de côté celles qui s'avèrent obsolètes pour enfin intégrer les nouveaux besoins. Mais dans ce processus déjà complexe, que faire des données existantes et comment les adapter à la nouvelle structure ? Comment conserver la synchronisation des données entre les deux projets ? Nous verrons ensemble comment LaFourchette a choisi de répondre à ces problématiques dans le cadre de la refonte d’une de leur principale application de Symfony 2.0 vers Symfony 3.</dd>
</dl>

[Slides](https://slideshare.net/VincentCHALAMON/r2d2-to-bb8-60662855)  
~~Video~~

By [Vincent Chalamon](https://connect.sensiolabs.com/profile/vincentchalamon)  
![github](icon/github.png) [@vincentchalamon](https://github.com/vincentchalamon)  
![twitter](icon/twitter.png) [@vincentchalamon](https://twitter.com/vincentchalamon)

---

## PHP Meminfo ou la chasse aux memory leak

<dl>
  <dt>Description</dt>
  <dd>Les profilers tel que Blackfire.io ou Memprof permettent de connaitre les fonctions qui prennent ou libèrent de la mémoire. Mais visualiser ce que contient la mémoire PHP permet de mieux comprendre les origines des memory leaks. L'extension PHP Meminfo fournit une vue synthétique du nombre d'instances par classe en mémoire, la liste compléte des objets et autres structures avec les relations qui les lient (membre de classe, présence dans un tableau, etc...). L'accès à ces informations de liaisons permet de comprendre pourquoi un élément n'a pas été libéré de la mémoire en suivant les références qui continuent à pointer sur lui. Le talk commencera par expliquer les mécanismes de libérations de la mémoire (references counter, cyclic reference garbage collector) spécifique à PHP, les effets des memory leaks sur les performances applicatives, puis détaillera des cases studies de fuite mémoire dans des projets Symfony2 et de leur analyse avec meminfo, ainsi que leur résolution.</dd>
</dl>

[Slides](https://speakerdeck.com/bitone/hunting-down-memory-leaks-with-php-meminfo)  
~~Video~~

By [Benoit Jacquemont](https://connect.sensiolabs.com/profile/bit_one)  
![github](icon/github.png) [@BitOne](https://github.com/BitOne)  
![twitter](icon/twitter.png) [@BJacquemont](https://twitter.com/BJacquemont)

---

## Retour d'expérience Reactive Architecture et Microservices : Comment découpler mes applications ?

<dl>
  <dt>Description</dt>
  <dd>Démonstration des principes de Reactive Architecture (responsive, resilient, elastic, message driven) sur le découpage d'une application en transition vers une architecture micro-services. Mise en place de Redis et des composants de Middleware (ESB, RabbitMQ) pour faciliter le découpage applicatif. Mutualisation des modèles canoniques pour éviter la duplication de code. Nous accompagnerons notre présentation d'exemples contextuels inspiré par la mise en œuvre de ces concepts chez Auchan E-Commerce</dd>
</dl>

[Slides](http://fabien.meurillon.org/sfLive2016/)  
~~Video~~

By [Fabien Meurillon](https://connect.sensiolabs.com/profile/fabienm)  
![github](icon/github.png) [@FabienM](https://github.com/FabienM)  
![twitter](icon/twitter.png) [@FabienM](https://twitter.com/FabienM)

---

## Le reveil du Workflow

<dl>
  <dt>Description</dt>
  <dd>Il est courant de gérer des statuts ou états de produits, dans des sites e-commerce ou éditoriaux. Pour ce faire, il est possible d'agir de façon classique, c'est-à-dire manuellement, ou d'avoir recours à des librairies qui proposent déjà des bases de code. Pour cette présentation, nous aborderons la notion de machine à état et sa définition avant d'envisager, son application, en examinant les librairies open sources existantes. Enfin, à la lumière de Symfony, nous étudierons le nouveau composant "Workflow"</dd>
</dl>

[Slides](https://speakerdeck.com/lyrixx/le-reveil-du-workflow)  
~~Video~~  
[Demo](https://github.com/lyrixx/SFLive-Paris2016-Workflow)

By [Grégoire Pineau](https://connect.sensiolabs.com/profile/lyrixx)  
![github](icon/github.png) [@lyrixx](https://github.com/lyrixx)  
![twitter](icon/twitter.png) [@lyrixx](https://twitter.com/lyrixx)

---

## ElasticSearch chez BlaBlaCar

<dl>
  <dt>Description</dt>
  <dd>Vous avez certainement entendu parler d'ElasticSearch auparavant. Chez BlaBlaCar nous adorons ce moteur de recherche et nous n'hésitons pas une seconde à l'utiliser lorsque cela est justifié. Recherches de trajets, FAQ, logs, détection de fraude, vous découvrirez la quasi intégralité des besoins qui ont justifiés la mise en place d'ElasticSearch chez BlaBlaCar.</dd>
</dl>

[Slides](https://speakerdeck.com/odolbeau/elasticsearch-chez-blablacar)  
~~Video~~

By [Olivier Dolbeau](https://connect.sensiolabs.com/profile/odolbeau)  
![github](icon/github.png) [@odolbeau](https://github.com/odolbeau)  
![twitter](icon/twitter.png) [@odolbeau](https://twitter.com/odolbeau)

---

## Performance au quotidien dans un environnement Symfony

<dl>
  <dt>Description</dt>
  <dd>C'est bien connu, les frameworks full stack, c'est lourd et c'est lent, Symfony le premier. Et chez CCM Benchmark (2ème groupe internet français - 50M de VU), on fait tout pour éviter la lenteur ! Alors pourquoi ai-je décider de migrer nos dizaines d'applications vers Symfony ? Et surtout comment respecter les critères de performances que nous avions défini avec notre bon vieux framework maison ? Voyons ensemble les raisons qui m'ont poussé à faire ce choix et surtout quels process et solutions nous avons pu mettre en oeuvre pour éviter des régressions de performance.</dd>
</dl>

[Slides](https://slideshare.net/xavierleune/performance-au-quotidien-dans-un-environnement-symfony)  
~~Video~~

By [Xavier Leune](https://connect.sensiolabs.com/profile/romainkuzniak)  
![github](icon/github.png) [@xavierleune](https://github.com/xavierleune)  
![twitter](icon/twitter.png) [@beoneself](https://twitter.com/beoneself)

---

## Keynote : Pourquoi se faire confiance ?

[Slides](https://speakerdeck.com/openclassrooms/pourquoi-se-faire-confiance)  
~~Video~~

By [Mathieu Nebra](https://connect.sensiolabs.com/profile/mateo21)  
![github](icon/github.png) [@mateo21](https://github.com/mateo21)  
![twitter](icon/twitter.png) [@m_nebra](https://twitter.com/m_nebra)

---

## PSR-6 & Symfony Cache : de la perf en standard

<dl>
  <dt>Description</dt>
  <dd>Après plusieurs mois de discussion, le PHP-FIG (PHP Framework Interop Group) a publié la PSR-6. Son objectif est de permettre l'interopérabilité entre implémentations de systèmes de mise en cache - un aspect indispensable pour gagner en performance dans votre application. Lors de cette conférence, nous verrons les avantages et les limites de PSR-6, nous discuterons des différentes solutions de cache existantes (Doctrine, Stash, php-cache), et je vous présenterai le nouveau composant Symfony Cache.</dd>
</dl>

~~Slides~~  
~~Video~~

By [Nicolas Grekas](https://connect.sensiolabs.com/profile/nicolas-grekas)  
![github](icon/github.png) [@nicolas-grekas](https://github.com/nicolas-grekas)  
![twitter](icon/twitter.png) [@nicolasgrekas](https://twitter.com/nicolasgrekas)

---

## Sécurité web: pirater pour mieux protéger

<dl>
  <dt>Description</dt>
  <dd>Il existe beaucoup de concepts dans la sécurité web, les maîtrisez-vous vraiment ? Pouvez-vous les utiliser afin de pirater un site ? Pourtant, pour toute faille que vous saurez exploiter, vous connaîtrez naturellement les moyens vous en protéger. Durant cette présentation, je vais vous montrer comment exploiter et se protéger de quelques vulérabilités: comment retrouver des mots de passes dans une base encodée en sha512, comment trouver et exploiter des failles XSS, bruteforcer une page de login, utiliser le clickjacking, outrepasser une vérification par SMS...</dd>
</dl>

[Slides](https://github.com/ninsuo/slides/blob/d65cf3fd216858e76116beea01cd4d7656bfb470/Web%20Security%20%28detailed%29%20[EN].pptx)  
~~Video~~

By [Alain Tiemblo](https://connect.sensiolabs.com/profile/ninsuo)  
![github](icon/github.png) [@ninsuo](https://github.com/ninsuo)  
![twitter](icon/twitter.png) [@ninsuo](https://twitter.com/ninsuo)

---

## Aller plus loin avec Doctrine2

<dl>
  <dt>Description</dt>
  <dd>La présentation a pour but de revenir sur différents aspects avancés de Doctrine mis en oeuvre au sein de projets Symfony 2.x/3. Elle abordera, entre autres, les éléments suivants : Étendre le vocabulaire DQL (spécifiquement ou à l'aide de bundles existants) Utiliser les différents listeners existants (annotations, listeners, subscribers, utilisation de l'UOW de Doctrine lors d'un flush, etc.); Créer des hydrateurs spécifiques ou des entités partielles pour améliorer les performances sur certaines opérations; Astuces diverses pour améliorer les performances (désactivation des logs, etc.)</dd>
</dl>

[Slides](http://blog.webnet.fr/wp-content/uploads/2016/04/2016-04-06-FINAL-Pr%C3%A9sentation-SymfonyLive-Doctrine2.pdf)  
~~Video~~

By [André Tapia](https://connect.sensiolabs.com/profile/dedeparisg)  
![github](icon/github.png) [@dedeparisg](https://github.com/dedeparisg)  
![twitter](icon/twitter.png) [@dedeparisg](https://twitter.com/dedeparisg)

---

## Refondre un moteur de règles avec l'expression language de symfony2

<dl>
  <dt>Description</dt>
  <dd>Présentation du métier de SELLSecure et de la couche technique du projet. Limitations du moteur historique: Augmentation de la complexité des règles demandées par le métier, temps de réponse plus adaptés aux exigences des clients, dette technique énorme sur ce composant essentiel. Choix de l'expression language: Recherche d'alternative dans le monde PHP et au dehors. Le composant Expression Language paraissait le plus convaincant; Permet de créer des règles complexes, le code est directement dans l'application et les temps de réponse semblaient bon. Mise en place: Migration des règles historiques, adaptation du code de l'application avec l'expression language; Extension de l'expression language pour implémenter certaines règles métiers. Démo. Conclusion, retour d'expérience: Tests de performances, retours des métiers et point sur la dette technique.</dd>
</dl>

[Slides](https://speakerdeck.com/husseinab/expression-language-symfony-live)  
~~Video~~

By [Hussein Abbas](https://connect.sensiolabs.com/profile/habbas)

---

## Sécurité et HTTP

<dl>
  <dt>Description</dt>
  <dd>Si autrefois nous ne nous soucions guère de la sécurité dans nos applications, il serait aujourd'hui impensable de se lancer dans le développement d'une application sans prendre en compte la sécurité vis à vis d'HTTP. Sans parler des outils communément utilisés dans Symfony (csrf_token, auto escaping Twig, escaping de commandes, hashage de données...), cette présentation s'attachera à présenter les différentes possibilités (CSP, HSTS, Framing options, etc...) offertes par les navigateurs et qu'il est facile a mettre en oeuvre dans Symfony via des bundles ou de la configuration pour éliminer de nombreux vecteurs d'attaque comme les DNS, le CDN poisoning ou les XSS.</dd>
</dl>

[Slides](https://speakerdeck.com/romain/securite-and-http-at-symfony-live-paris-2016)  
~~Video~~

By [Romain Neutron](https://connect.sensiolabs.com/profile/romain)  
![github](icon/github.png) [@romainneutron](https://github.com/romainneutron)  
![twitter](icon/twitter.png) [@romainneutron](https://twitter.com/romainneutron)

---

## Construire des applications cloud natives

<dl>
  <dt>Description</dt>
  <dd>Ces-jours-ci on ne parle que de montée en échelle et de scalabilité horizontale. Dans cette présentation, un peu abstraire mais bien pratique, nous parlerons des choix architecturaux que vous pouvez faire pour rendre votre application prête pour un succès planétaire (dommage d’échouer an ayant réussi). Nous allons parler de micro-services, de leur utilité et leurs limites, là où l’on veut communiquer par JSON/HTTP (que d’autres appels REST) et là où un Message Queue en bonne et due forme vous rendra des fiers services futurs. Nous parlerons aussi des écueils à éviter (par la séparation des domaines écritures / lectures) et des choses, que jamais ô jamais vous ne devriez mettre dans une base de données relationnelle. Nous évoquerons en guise de travaux pratiques et cerise sur le gateau comment faire des migration paresseuses avec Symfony.</dd>
</dl>

[Slides](http://fr.slideshare.net/OriPekelman/construire-des-applications-cloud-natives-symfonylive-paris-2016)  
~~Video~~

By [Ori Pekelman](https://connect.sensiolabs.com/profile/jpetitcolas)  
![github](icon/github.png) [@OriPekelman](https://github.com/OriPekelman)  
![twitter](icon/twitter.png) [@OriPekelman](https://twitter.com/OriPekelman)

---

---

---

# Lightning Talks

## "S" is for "Secure"

[Slides](http://slides.com/jeremyderusse/deck-9)  
~~Video~~

By [Jérémy Derussé](https://connect.sensiolabs.com/profile/jderusse)  
![github](icon/github.png) [@jeremy-derusse](https://github.com/jeremy-derusse)  
![twitter](icon/twitter.png) [@jderusse](https://twitter.com/jderusse)

---

## HTTPS automatiquement et gratuitement dans vos projets Symfony

[Slides](https://speakerdeck.com/tgalopin/https-automatiquement-et-gratuitement-dans-vos-projets-symfony)  
~~Video~~  
[ACME PHP](https://github.com/acmephp)

By [Titouan Galopin](https://connect.sensiolabs.com/profile/tgalopin)  
![github](icon/github.png) [@tgalopin](https://github.com/tgalopin)  
![twitter](icon/twitter.png) [@titouangalopin](https://twitter.com/titouangalopin)

---

## Persister des Value Objects avec Doctrine

[Slides](https://speakerdeck.com/hhamon/persister-des-value-objects-avec-doctrine)  
~~Video~~

By [Hugo Hamon](https://connect.sensiolabs.com/profile/hhamon)  
![github](icon/github.png) [@hhamon](https://github.com/hhamon)  
![twitter](icon/twitter.png) [@hhamon](https://twitter.com/hhamon)
