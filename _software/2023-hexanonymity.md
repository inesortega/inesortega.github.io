---
title: "Hexanonymity: a scalable geo-positioned data clustering algorithm for anonymisation purposes"
collection: software
type: "software"
permalink: /software/2023-hexanonymity
url: https://github.com/Gradiant/Hexanonymity
date: 2023-03-09
---

Hexanonymity is a new algorithm for the anonymisation of geo-positioned data which introduces a limited amount of information loss while providing k-anonymity. Hexanonymity leverages the Uber H3 geo-indexing system, which subdivides the earth into hexagonal meshes. We take advantage of a property of hexagon meshes, where for any of them, the distance from its centre to the centre of the six surrounding hexagons is always the same. This property allows the algorithm to generate high-quality clusters of geo-positioned data points, introducing a limited information loss.

Hexanonymity therefore provides k-anonymity to datasets of geo-positioned datapoints. We use the Uber H3 library to group the set of locations into recursively larger areas so that, at the end of the process, locations belonging to the same cell in the hierarchy report the same final location, becoming indistinguishable and providing k-anonymity.

The full methodology is explained in the [Hexanonymity paper](https://ieeexplore.ieee.org/abstract/document/10190642).