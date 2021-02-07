---
layout: post
title: "MPI vs OpenMPI vs OpenMP"
categories: misc
---

Pawan Ghildiyal has a great post on explaing the MPI, OpenMPI, and OpenMP (https://pawangh.blogspot.com/2014/05/mpi-vs-openmp.html?showComment=1612658047228#c2803165219350581253). Below are just some bullet points summarized from this post to help me memorize:

- OpenMPI is a particular API of MPI, same as MPICH, HP-MPI, Intel MPI

- OpenMP stand for Open Multiprocessing, a shared memory standard which is basically an add on in compiler (available on gcc and intel compiler).

- MPI target on both distributed and share memory system, based on both process and thread based approach 

- Openmp target on shared memory system, based on thread approach


