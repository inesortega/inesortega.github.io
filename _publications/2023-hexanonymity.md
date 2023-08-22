---
title: "Hexanonymity: a scalable geo-positioned data clustering algorithm for anonymisation purposes"
collection: publication
permalink: /publication/2023-jnic2023-lstm-ueba
date: 2023-07-31
venue: '2023 IEEE European Symposium on Security and Privacy Workshops (EuroS&PW)'
type: "conference"
paperurl: 'https://ieeexplore.ieee.org/abstract/document/10205609/'
citation: 'J. Rodriguez-Viñas, I. Ortega-Fernandez and E. S. Martínez, "Hexanonymity: a scalable geo-positioned data clustering algorithm for anonymisation purposes," 2023 IEEE European Symposium on Security and Privacy Workshops (EuroS&PW), Delft, Netherlands, 2023, pp. 396-404, doi: 10.1109/EuroSPW59978.2023.00050.'
---
Advances in sensors, trackers and positioning systems had led to the emergence of multiple locationbased services (LBS), resulting in multiple devices and users reporting their precise position and raising many privacy concerns. Anonymisation of geo-positioned data can provide a high level of privacy to the end users, but usually at the cost of introducing high levels of information loss on the location reported to the LBS. This paper presents Hexanonymity, a new algorithm for the anonymisation of geo-positioned data which introduces a limited amount of information loss while providing k-anonymity. Hexanonymity leverages the Uber H3 geo-indexing system, which subdivides the earth into hexagonal meshes. We take advantage of a property of hexagon meshes, where for any of them, the distance from its centre to the centre of the six surrounding hexagons is always the same. This property allows the algorithm to generate high-quality clusters of geo-positioned data points, introducing a limited information loss. This new algorithm improves the current state-of-the-art in terms of the quality of the anonymised data points while providing a similar level of privacy, with a percentage of anonymised locations reduced by only 0.503% when compared to Adaptive Interval Cloaking. Hexanonymity leverages geo-indexing systems to offer a scalable approach to the anonymisation of geo-positioned data in linear time, suitable for big data and real-time scenarios.

[Download paper here](https://doi.org/10.1109/EuroSPW59978.2023.00050)