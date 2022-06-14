---
layout: post
permalink: /matematica/poliedos-prismas
title: "Poliedros e Primas"
author: Rebecca
---

# Poliedros
## O que são poliedros?
Poliedro é todo sólido geométrico que são formados por superfícies planas, e cada uma dessas superfícies chamamos de **faces**, e cada uma dessas faces é um polígono.

## Poliedros convexos e não convexos
{% raw %}
<canvas id="hexagon"></canvas>
<style>
  #hexagon { border: thin dashed red; }
</style>
<script>
  var ctx = document.getElementById('hexagon').getContext('2d');

// hexagon
var numberOfSides = 6,
    size = 20,
    Xcenter = 25,
    Ycenter = 25;

ctx.beginPath();
ctx.moveTo (Xcenter +  size * Math.cos(0), Ycenter +  size *  Math.sin(0));          

for (var i = 1; i <= numberOfSides;i += 1) {
  ctx.lineTo (Xcenter + size * Math.cos(i * 2 * Math.PI / numberOfSides), Ycenter + size * Math.sin(i * 2 * Math.PI / numberOfSides));
}

ctx.strokeStyle = "#000000";
ctx.lineWidth = 1;
ctx.stroke();
</script>
 {% endraw %}
