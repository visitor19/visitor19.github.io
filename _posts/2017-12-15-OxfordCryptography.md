---
title: "Post Quantum Cryptography "
date: 2017-12-15
tags: [journal]
excerpt: "Thoughts after spending a few days at Oxford University attending the IMA conference on Cryptography and Coding."
mathjax: true
---

[Draft] I spent a few days at St Catherine's college, Oxford University attending the Institute of Mathematics and Applications' conference on Cryptography and Coding. My focus of interest was on post quantum cryptography.

Our digital information is almost exclusively protected by cryptographic algorithms which rely on mathematical operations which are computationally easy to execute but who's inverses are computationally hard problems. Specifically, multiplying two large prime numbers is easy yet taking the resultant product and obtaining it's prime factorisation is hard. Cryptography thus relies on on the fact that the only available attack vector, a brute force attack, will take far longer to execute then time that the data needs to be kept confidential. This typically could be in the order of thousands, millions or billions of years.

The above is proven technology with only two weaknesses. Firstly their could be an advancement in the underlying areas of mathematics makes what was a computationally hard problem no longer such. And secondly, the above discussion is in terms of classical computing only. Quantum computing is now a reality and this threatens to make traditional cryptography insecure to those who possess it. 1994 Shor's algorithm proposed a quantum computing approach to the prime factorisation integers and from 2001 onwards it has been demonstrated using emergent quantum technologies. The key point to note is the computing complexity of the problem which is NP-Hard in classical computing is reduced to polynomial time N log N.

In Oct 2017 Bristol's quantum engineering department put the bound on the quantum singularity at 50 photons. This milestone denotes the point at which quantum computing will outperform classical algorithms. It is uncertain when the worlds information encrypted using classical methods such as RSA, DES, etc will become insecure but it is reasonable to assume that date lies within the next 15 years.

While the field of Quantum engineering is looking at novel ways to secure information of the future using the properties of quantum mechanics itself (e.g Quantum Key Distribution), Mathematical research groups are focused on how to provide security to classical computing in a post quantum age.

Modern classical cryptographic alternatives have and are being researched, including Lattice based encryption schemes, Homomorphic based encryption and Individual
