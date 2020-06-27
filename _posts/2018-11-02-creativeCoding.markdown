---
layout: post
title:  Creative Coding Experiments
date:   2018-11-02 14:57:00 -0600
category: posts
permalink: /posts/creative-coding
---
During my front-end tech learning phase a few years ago, I stumbled upon world of creative coding / generative art. I watched *[CodingTrain](https://www.youtube.com/user/shiffman/featured "Open YouTube Link"){:target="_blank"}* by Dan Shiffman where he shares his incredible knowledge around processing framework.  

Fascinated by Dan's work, while exploring on the interweb I came across and completed Matt Deslauriers's course on *[FrontEndMasters](https://frontendmasters.com/courses/canvas-webgl/ "Open FrontEndMasters"){:target="_blank"}* thorugh which I learnt fundamental concepts behind creative development work.   

Here's a code snippet used for following generative samples using *[Canvas-Sketch](https://github.com/mattdesl/canvas-sketch.git "Open GitHub Repo"){:target="_blank"}* framework by Matt.

    const createGrid = () => { //creates a grid using u, v co-ordinate system
      const points = [];
      const count = 40;
      for (let x = 0; x < count; x++) {
        for (let y = 0; y < count; y++) {
          const u = count <= 1 ? 0.5 : x / (count - 1);
          const v = count <= 1 ? 0.5 : y / (count - 1);
          const radius = Math.abs(random.noise2D(u, v)) * 0.2;
          points.push({
              //specified an object with radius & position randomness
              color: random.pick(palette),
              radius,
              rotation: random.noise2D(u, v),
              position: [u, v]
          });
        }
      }
      return points;
    };
  
<br>Following images are a result of iterations using canvas-sketch library.   

<div style="
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 10px;
">
  <img src="/assets/media/gen-art/genArt1.png" alt="genArt3"/>
  <img src="/assets/media/gen-art/genArt2.png" alt="genArt2"/>
  <img src="/assets/media/gen-art/genArt4.png" alt="genArt4"/>
  <img src="/assets/media/gen-art/genArt3.png" alt="genArt1"/>
</div>
  
<!-- # GLSL Shader
<img src="/assets/img/genArt5.png" alt="genArt5"/> -->
