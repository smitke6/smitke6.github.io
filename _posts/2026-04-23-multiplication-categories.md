---
layout: post
title: "Multiplying natural numbers: commutativity and two categorifications"
date: 2026-04-23
---

When we first encounter natural numbers, we don't immediately meet their abstract form. Instead, we are introduced to their more "natural" aspect: a *categorification* of the natural numbers via the category $\mathbf{FSet}$ of finite sets. 

You can think of these as sets of apples. To simplify, we can even restrict ourselves to the full subcategory containing exactly one set of each size—let's call it the "category of sets of apples," or $\mathbf{AppleSet}$. Decategorification maps a finite set to its cardinality (a natural number), and as we learn early on, the decategorification of a disjoint union is simply addition.

So, how do we categorify multiplication? 

One option is the Cartesian product of sets. This works, but it's a more advanced concept and perhaps less "natural" for elementary school students. Instead, our first encounter with multiplication is usually framed as the action of the monoid $\mathbb{N}$ on the category $\mathbf{AppleSet}$ (for simplicity, we only need to look at the action on objects here). Any natural number $n$ maps a set in $\mathbf{AppleSet}$ to its disjoint union with itself $n$ times. 

Notice that the monoid $\mathbb{N}$ plays two fundamentally different roles here: first, as the decategorification of $\mathbf{AppleSet}$ (counting the apples in a set), and second, as the operator acting on $\mathbf{AppleSet}$ via disjoint unions.

From this perspective, it is not at all obvious that these two $\mathbb{N}$ monoids should be thought of as "the same thing." It is even less obvious why multiplication (the decategorification of the monoid action on $\mathbf{AppleSet}$) is *commutative*—even after we establish an isomorphism between the two monoids and identify their elements with one another. 

Or, as I might have phrased it as a first-grader:

> *"Wait... why is three times five the exact same as five times three? I checked, and it works, but it feels like a coincidence."*

We can, of course, prove commutativity: "Three times five" is the disjoint union of three sets—$A$, $B$, and $C$—each containing five apples. If we look at this disjoint union, "remember" where each apple came from, and redistribute them, we can build new sets of three, each containing exactly one apple from $A$, $B$, and $C$. 

But this is actually cheating! I covertly passed through the Cartesian product categorification of multiplication, which easily shows why multiplication is commutative. This implies that the Cartesian product inherently contains more information than the monoid action (where "five times three" is strictly "five instances of three").

I don't pretend to offer a "solution" to this pedagogical problem (if it even is one—it might just be in my head!). I mostly just wanted to offer some food for thought.
<script async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>
