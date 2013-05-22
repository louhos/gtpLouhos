---
title       : R, avoin data ja toistettavat analyysit 
subtitle    : Geoinformatiikan tutkimuspäivät 2013
author      : Joona Lehtomäki 
job         : Louhos
license     : by-sa
github      :
  user        : louhos
  repo        : gtpLouhos
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

--- &vcenter

## Hei!

<div class="row">
  <div class="span3">
    <img src="assets/img/joona_sunglasses.jpg" class="presenter"/>
    <h3 style="text-align: center;">
      <a href="https://twitter.com/jlehtoma">@jlehtoma</a>
    </h3>
  </div>
  <div class="span7">
  <ol>
    <li> 
      Helsingin yliopisto, biotieteiden laitos, <a href="http://cbig.it.helsinki.fi/people/#joona-lehtomaki">Conservation Biology Informatics Group</a>
    </li>
    <li>
      Suomen ympäristökeskus, <a href="http://goo.gl/8O1GB">luontoympäristökeskus</a>
    </li>
    <li>
      <a href="http://louhos.github.io/">Louhos</a>-yhteisö
    </li>
    </ol>
  
  </div>
</div>

--- bg:url(assets/img/louhos_admins.png) bg-repeat:no-repeat bg-position:center

--- #louhos-intro &notitle bg:black

<iframe src="http://louhos.github.io/">O-ou, ei onnistu...</iframe>

--- #title-toistettavuus &vcenter

<span class="gigantic">Toistettavuus</span>

--- #data-to-action &vcenter

<img src="assets/img/data_to_action.png" />

--- #gradu-workflow bg:url(assets/img/gradu_workflow.png)

--- #problem-1

## Ongelma tutkimuksessa?

Toistettavuus:
> 1. "Allows others to build upon existing work and use it to test new ideas and develop methods" 
(<a href="http://www.scfbm.org/content/8/1/7">Ram, 2013</a>)
> 2. "While currently there is unilateral emphasis on 'first' discoveries, there should be as much emphasis on replication of discoveries" (<a href="http://www.telegraph.co.uk/technology/3342867/Is-the-spirit-of-Piltdown-man-alive-and-well.html">Ioannidis, 2005</a>)

--- #problem-2 &vcenter

## Ongelma päätöksenteossa?

<img src="http://www.nextnewdeal.net/sites/default/files/styles/large/public/content_images/reinhart_rogoff_coding_error_0.png" />

Reinhart & Rogoff, "<a href="http://www.nber.org/papers/w15639.pdf">Growth in a Time of Debt</a>"  
<span class="source">Kuvan lähde: <a href="http://www.nextnewdeal.net/rortybomb/researchers-finally-replicated-reinhart-rogoff-and-there-are-serious-problems">Next New Deal</a></span>

--- #title-toistettavuus &vcenter

<span class="gigantic">R</span>

--- #R-intro1 bg:url(assets/img/R_command_line.png) bg-repeat:no-repeat bg-position:center

--- #R-intro2 &vcenter

<div class="row">
  <div class="span2">
    <img src="http://www.lindinglab.org/external-files/images/Rlogo1.png/image" height="125" / >
  </div>
  <div class="span8">
    <h2><a href="http://cran.r-project.org">http://cran.r-project.org</a></h2>
  </div>
</div>

* Vuorovaikutteinen ja modulaarinen (avoin data, tilastotiede, visualisointi)
* Tuhansia analyysimenetelmiä
* Grafiikkaominaisuudet
* Avoin lähdekoodi sekä laaja käyttäjä- ja kehittäjäyhteisö

--- #R-intro3 &vcenter

<img src="http://r4stats.files.wordpress.com/2012/04/fig_7a_scholarlyimpactbig61.png" />

Analyysiohjelmien akateeminen käyttö (Google Scholar)  
<span class="source">Lähde: <a href="http://r4stats.com/2013/05/14/beginning-of-the-end-v2/">r4stats.com</a></span>

--- #R-intro4 &vcenter

<img src="http://r4stats.files.wordpress.com/2012/04/fig_1a_listserv11.png" />

Liikenne sähköpostilistoilla (listerv)  
<span class="source">Lähde: <a href="http://r4stats.com/2013/05/14/beginning-of-the-end-v2/">r4stats.com</a></span>

--- #R-intro5 &vcenter

<img src="http://r4stats.files.wordpress.com/2012/04/fig_1b_forums.png" height="500"/>

Kysymysten määrä eri foorumeilla 10.2.2013  
<span class="source">Lähde: <a href="http://r4stats.com/2013/05/14/beginning-of-the-end-v2/">r4stats.com</a></span>

--- #r-ecosystem bg:url(assets/img/ecosystem.jpg) bg-repeat:no-repeat bg-position:center

<span class="attribution">Photo by premus on <a href="http://www.fotopedia.com/items/flickr-2677729640">Flickr</a>, CC-BY</span>

--- #r-ecosystem2 &vcenter

<img src="assets/img/tech_logos.png" />

--- #r-ecosystem3 &vcenter

<img src="assets/img/toistettava_analyysi_web.png" />  
<span class="source">Lähde: <a href="http://markuskainu.fi/r-tutorial/repro/suomeksi.html">Markus Kainu</a></span>

--- #source &vcenter

<a href="https://github.com/louhos/gtpLouhos"><img src="http://octodex.github.com/images/collabocats.jpg" height="400" /></a>  
Esityksen lähdekoodi

--- #xkcd &vcenter

<img src="assets/img/tar.png" /> 

<span class="source">Lähde: <a href="http://xkcd.com/1168/">XKCD 1168</a></span>

--- #title-sorvi &vcenter

## Toistettavuus + R + avoin data =   
<span class="gigantic" style="">sorvi ja datawiki</span>

--- #sorvi-intro &vcenter

## <span class="orange">sorvi</span> - suomalaisen avoimen datan R-paketti

> 1. <span class="emphasis">Datan saatavuus</span> joustavat datan haku- ja putsausrutiinit
> 1. <span class="emphasis">Läpinäkyvyys ja toistettavuus</span> kaikki vaiheet yhdessä koodissa
> 1. <span class="emphasis">Uusia tutkimusvälineitä</span> sovelluksia täydentämään
> 1. <span class="emphasis">Vuorovaikutteisuus</span> nopea datan seulonta ja visualisointi
> 1. <span class="emphasis">Lokalisoitu</span> kotimaisiin tarpeisiin

--- #datawiki-intro &vcenter

## <span class="orange">datawiki</span> - esimerkkeihin perustuva dataopas

> 1. <span class="emphasis">Datakatalogi</span> mukana n. 20 kotimaista tietolähdettä
> 1. <span class="emphasis">Käyttöesimerkit</span> toistettavat esimerkit sorvilla
> 1. <span class="emphasis">Kehittäjäyhteisön tuki</span> kaikki voivat osallistua

--- #kuntajako-1 &vcenter

## Uusi kuntajako: yhdistely ja visualisointi

<div class="row">
  <div class="span2">
    <img src="assets/img/logo_kuntajako.png" / >
  </div>  
  <div class="span8">
    <div class="span3">
      <img src="assets/img/uusi_kuntajako.png" / >
    </div>
    <div class="span3">
      <img src="assets/img/uusi_kuntajako_2.png" / >
    </div>
  </div>
</div>

<span class="source">Lähde: <a href="https://louhos.wordpress.com/2012/02/26/uuden-kuntajaon-mukainen-kuntien-yhdistaminen-ja-visualisointi/">Louhos-blogi</a></span>

--- #kuntajako-2 bg:url(assets/img/datawiki_kuntajako.png) bg-repeat:no-repeat bg-position:center

--- #r-ecosystem2 bg:black

<iframe src="http://sorvivalas.com:8787/  ">O-ou, ei onnistu...</iframe>

--- #hsy-pks-1 &vcenter

## HSY:n väestöruudukko pääkaupunkiseudulla

<div class="row">
  <div class="span2" style="padding-top: 65px;">
    <img src="assets/img/logo_hsy.png" / >
  </div>  
  <div class="span8">
    <img src="assets/img/hsy_pks.png" / >
  </div>
</div>

--- #kuntajako-2 bg:url(assets/img/datawiki_hsy.png) bg-repeat:no-repeat bg-position:center

--- #summary &vcenter

<span class="moderate">Toistettavuus ja läpinäkyvyys</span>  
paranee kun avaamme ja jaamme  
<br />
<br />
<span class="moderate blue" style="padding-left:1em">dataa</span>
<span class="moderate blue" style="padding-left:1em">koodin</span>
<span class="moderate blue" style="padding-left:1em">osaamista</span>

--- #kuntajako-2 bg:url(assets/img/kiitos.png) bg-repeat:no-repeat bg-position:center
