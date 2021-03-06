---
layout: page
title: Archiefviewer op de kaart
---
# Archiefviewer op de kaart

Als experiment voor een gebied binnen de gemeente Lisse hebben we veldwerken (minimaal 100 jaar oud) gelinkt aan de percelen, en deze via een viewer beschikbaar gemaakt.

Voor lang niet alle percelen is er een oud veldwerk beschikbaar, dus klik vooral op lage perceelsnummers (bv. 2101).

<link rel="stylesheet" href="/assets/openlayers/v4.6.5-dist/ol.css" type="text/css">
<!-- The line below is only needed for old environments like Internet Explorer and Android 4.x -->
<script src="https://cdn.polyfill.io/v2/polyfill.min.js?features=requestAnimationFrame,Element.prototype.classList,URL">
</script>
<script src="/assets/openlayers/v4.6.5-dist/ol.js">
</script>
<style>
  .map:-moz-full-screen {
    height: 100%;
  }
  .map:-webkit-full-screen {
    height: 100%;
  }
  .map:-ms-fullscreen {
    height: 100%;
  }
  .map:fullscreen {
    height: 100%;
  }
  .ol-rotate {
    top: 3em;
  }
  .map {
    position: relative;
  }
  #overlay {
    display: inline-block;
    position: absolute;
    top: 1em;
    right: 3em;
    height: 90%;
    width: 300px;
    z-index: 20000;
    background-color: white;
    padding: 0 0.5em 0.5em 0.5em;
    opacity: 0.8;
    overflow-y: auto;
  }
</style>

<div id="map" class="map">
  <div id="overlay" style="z-index:9999">Selecteer een perceel</div>
</div>
<script src="archive-mapviewer.js"></script>
