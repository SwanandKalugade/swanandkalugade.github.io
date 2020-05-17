---
layout: post
title:  Creative Coding
date:   2018-11-02 14:57:00 -0600
categories: code
permalink: /code/creative-coding
---
During my front-end tech learning phase a few years ago, I stumbled upon world of creative coding / generative art. I watched *[CodingTrain](https://www.youtube.com/user/shiffman/featured "Open YouTube Link"){:target="_blank"}* by Dan Shiffman where he shares his incredible knowledge around processing and p5.js.  

<br>
Code snippet from [`Canvas-Sketch`](https://github.com/mattdesl/canvas-sketch.git "Open GitHub Repo"){:target="_blank"} framework by Matt Deslauriers.

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
  
<br>Following images are results using canvas-sketch library and GLSL Shaders.  

<img src="/assets/img/genArt3.png" alt="genArt3"/>
<img src="/assets/img/genArt2.png" alt="genArt2"/>
<img src="/assets/img/genArt1.png" alt="genArt1"/>
<img src="/assets/img/genArt4.png" alt="genArt4"/>

  
# GLSL Shader
<img src="/assets/img/genArt5.png" alt="genArt5"/>