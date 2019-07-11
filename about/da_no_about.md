---
layout: page
title: About Neodroid Danish/Norwegian
tags: [about, Jekyll, theme, moon]
date: 2018-11-13
comments: false
---

Neodroid is a reinforcement learning and data generation, enabling platform for games and research.


Beskrivelse
Neodroid platform er bygget til at supportere en process af prototype bygning og experimentation med 
reinforcement learning, men kan med fordel også bruges til at kompilere dataset til andre læringsparadigmer.

Til supervised computer vision problemmer, kan man med fordel udnytte Neodroids allerede implementeret funktionalitet til at lave domænerandomisering, igennem permutioner af lysforhold, overflade teksture, størrelser, rotationer og meget mere.

Platformen har 2 essentielle dele
Unity delen (Kodenavn: Droid) 
Python delen (Kodenavn: Neo)
Unity delen er en sæt værktøjer til hurtig prototypiing og konstruktion af simuleringsmiljøer til en reinforcement learning, implementation er centeret omkring en kontinuerlig interaktion med andre eksterne selvstændig process (med kommunikation over TCP, IPC, PGM med mere, hvad end ZeroMQ tillader).

En mulig opsætning er så at hver tidskridt en eksterne process vælge mellem et antal af muligheder for at påvirke simuleringen.

Python delen er så til at bygge den eksterne process, der skal tage beslutninger og observerer simuleringsmiljøet(F.eks. en verdenstilstand).

---

_[Neodroid](https://github.com/sintefneodroid) is developed with support from Research Council of Norway Grant #262900. ([https://www.forskningsradet.no/prosjektbanken/#/project/NFR/262900](https://www.forskningsradet.no/prosjektbanken/#/project/NFR/262900))_

---
