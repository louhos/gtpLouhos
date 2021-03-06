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
<div class="row">
  <div class="span9 offset1">

<ul>
<li>
Helsingin yliopisto, biotieteiden laitos, <a href="http://cbig.it.helsinki.fi/people/#joona-lehtomaki">Conservation Biology Informatics Group</a>
</li>
<li>
Suomen ympäristökeskus, <a href="http://goo.gl/8O1GB">luontoympäristökeskus</a>
</li>
<li>
<a href="http://louhos.github.io/">Louhos</a>-yhteisö
</li>
</ul>

  </div>
</div>

--- #louhos-intro &notitle bg:black

<iframe src="http://louhos.github.io/">O-ou, ei onnistu...</iframe>

--- bg:url(assets/img/louhos_admins.png) bg-repeat:no-repeat bg-position:center

--- #gradu-workflow bg:url(assets/img/gradu_workflow.png)

--- #problem

## Ongelma?
  
<br />
<br />
<span class="orange">**Tutkimuksessa**</span>

> Kuilu julkaisun ja toistettavuuden välillä

<span class="orange">**Päätöksenteossa**</span>

> Onko päätöksenteko palautettavissa aineistoon ja tutkimuksiin?

--- #R-intro1 bg:url(assets/img/R_command_line.png) bg-repeat:no-repeat bg-position:center

--- #R-intro2 &vcenter

<div class="row">
  <div class="span2" style="margin-bottom: 30px;">
    <img src="assets/img/R_logo.png" / >
  </div>
  <div class="span8">
    <h2><a href="http://cran.r-project.org">http://cran.r-project.org</a></h2>
  </div>
</div>

> * Avoimen lähdekoodin ohjelmointikieli ja tilastollisen laskennan ympäristö
> * Komentorivipohjainen ja vuorovaikutteinen 
> * Grafiikkaominaisuudet
> * Laaja käyttäjä- ja kehittäjäyhteisö
> * Rakenteeltaan modulaarinen ja laajennettavissa

--- #R-intro3 &vcenter

<img src="http://r4stats.files.wordpress.com/2012/04/fig_1a_listserv11.png" />

Liikenne sähköpostilistoilla (listerv)  
<span class="source">Lähde: <a href="http://r4stats.com/2013/05/14/beginning-of-the-end-v2/">r4stats.com</a></span>

--- #r-ecosystem bg:url(assets/img/ecosystem.jpg) bg-repeat:no-repeat bg-position:center

<span class="attribution">Photo by premus on <a href="http://www.fotopedia.com/items/flickr-2677729640">Flickr</a>, CC-BY</span>

--- #R-intro5 &vcenter

<span class="gigantic">6275</span>

<span class="source">Lähde: <a href="http://r4stats.com/2013/05/14/beginning-of-the-end-v2/">r4stats.com</a></span>

R-pakettien lukumäärä 19.3.2013

--- #r-ecosystem2 &vcenter

## R ja toistettavuus

<img src="assets/img/tech_logos.png" />

--- #markdown

<iframe src="http://markable.in/editor/">O-ou, ei onnistu...</iframe>

--- #r-ecosystem2 bg:black

<iframe src="http://sorvivalas.com:8787/  ">O-ou, ei onnistu...</iframe>

--- #r-ecosystem3 &vcenter

<img src="assets/img/toistettava_analyysi_web.png" />  
<span class="source">Lähde: <a href="http://markuskainu.fi/r-tutorial/repro/suomeksi.html">Markus Kainu</a></span>

--- #xkcd &vcenter

<img src="assets/img/tar.png" /> 

<span class="source">Lähde: <a href="http://xkcd.com/1168/">XKCD 1168</a></span>

--- #sorvi-intro &vcenter

## <span class="orange">sorvi</span> - suomalaisen avoimen datan R-paketti

> 1. <span class="emphasis">Datan saatavuus</span> joustavat datan haku- ja putsausrutiinit
> 1. <span class="emphasis">Läpinäkyvyys ja toistettavuus</span> kaikki vaiheet yhdessä koodissa
> 1. <span class="emphasis">Uusia tutkimusvälineitä</span> sovelluksia täydentämään
> 1. <span class="emphasis">Vuorovaikutteisuus</span> nopea datan seulonta ja visualisointi
> 1. <span class="emphasis">Lokalisoitu</span> kotimaisiin tarpeisiin

<span class="source">[http://louhos.github.io/sorvi/](http://louhos.github.io/sorvi/)</span>

--- #datawiki-intro &vcenter

## <span class="orange">datawiki</span> - dataopas esimerkkeihin 

> 1. <span class="emphasis">Datakatalogi</span> mukana n. 20 kotimaista tietolähdettä
> 1. <span class="emphasis">Käyttöesimerkit</span> toistettavat esimerkit sorvilla
> 1. <span class="emphasis">Kehittäjäyhteisön tuki</span> kaikki voivat osallistua

<span class="source">[http://louhos.github.io/datawiki](http://louhos.github.io/datawiki/index.html)</span>

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

--- #hsy-pks-1 &vcenter

## HSY:n väestöruudukko pk-seudulla

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
