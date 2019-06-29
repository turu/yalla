Table of Contents
=================

   * [About YALLA](#about-yalla-v030)
   * [What's the point](#whats-the-point)
   * [What's inside](#whats-inside)
      * [Stream processing](#stream-processing)
         * [Item filters](#item-filters)
   * [Should I use these implementations in production](#should-i-use-these-implementations-in-production)

# About YALLA v0.3.0
_**Y**et **A**nother **L**ame **L**ibrary of **A**lgorithms_* 
is an ever growing collection of algorithms and data structures 
used in **machine learning** and large scale **data processing**, 
implemented from scratch for fun and profit.

\* also see https://www.urbandictionary.com/define.php?term=yalla

# What's the point
As any field progresses, new tools and libraries are created 
to make our lives easier. They help us turn ideas into working 
products faster and with better quality. They achieve this thanks 
to an ever increasing level of abstraction. Unfortunately high 
level of abstraction comes with a cost. It becomes easy to miss 
or loose grasp of the inner workings of particular tools, 
models and algorithms.

This repository is an attempt to keep myself sharp and my feet 
firmly on the ground - to consolidate my understanding of 
the intuition behind these algorithms and encode it in the form 
of plain source code with minimal dependencies.

**To implement is to understand.**

# What's inside
Algorithms and data structures implemented in YALLA, are divided into packages and submodules
aligned with their real life domains and applications. Each comes with:
  * a (hopefully) clear and informative implementation
  * short documentation
  * small suite of sanity tests and
  * (optionally) an accompanying Jupyter notebook

Currently the following topics are covered:
## Stream processing
### Item filters
Algorithms to test for item uniqueness ("have I seen this item before?") in an infinite stream of data:
1. Bloom Filter
2. Cuckoo Filter
### Item counters
Algorithms to count the number of distinct, unique elements in an infinite stream of data:
1. HyperLogLog
### Stream moments
Algorithms to compute mean, variance & standard deviation, skewness and kurtosis of infinite streams of data:
1. Welford-Knuth-Pebay one-pass, parallel, statistical moments

# Should I use these implementations in production
![N|Solid](https://i.kym-cdn.com/entries/icons/mobile/000/005/180/YaoMingMeme.jpg)

**If you like to see the world burn, then yes. Otherwise, caution is advised.**

The source code of algorithms and data structures in this repository is not optimized for efficiency or accuracy. 
It is intentionally as pure and pseudo-code-like as possible. It may also ignore certain corner-cases for the sake of
simplicity. The primary purpose of this library is to serve as a repository of reference implementations, to aid and 
maintain understanding.  
