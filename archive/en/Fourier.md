---
layout: post
category: joke
title: "Ineffective Fourier transforms"
date: 2017-05-30
first_comment: "This table also appears in my doctoral thesis."
---

*(A joke inspired by [xkcd #1185](https://xkcd.com/1185))*

<div style="display: flex; flex-wrap: wrap; justify-content: space-between;">

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Lazy Fourier Transform (LFT)**<br>
For an input vector $ \mathbf{x} $:

1. Pad $ \mathbf{x} $ with zeros until its length is a power of 2.
2. Pad $ \mathbf{x} $ with more zeros until its length is a power of 3.
3. Give 'em a billion more zeros.
4. For a random prime $ p $, pad $ \mathbf{x} $ with more zeros until its length is a power of $ p $.
5. OK, now $ \mathbf{x} \equiv 0 $ approximately, hence its Fourier transform is the zero vector, so just return zero.

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Slow Fourier Transform (SFT)**<br>
For an input vector $ \mathbf{x} $:

1. Initialize $ \mathbf{y}=0 $.
2. Find a Gaussian fit for $ \mathbf{x} $.
3. The Fourier transform of a Gaussian is a Gaussian! Add the transformed Gaussian to $ \mathbf{y} $, and subtract the original Gaussian from $ \mathbf{x} $.
4. Repeat until $ \mathbf{x}=0 $, and then return $ \mathbf{y} $.

**Complexity:** I dunno, does it even converge?

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Quantum Fourier Transform (QFT)**

1. Wait until they build a good enough quantum computer with a large number of qubits.
2. Run the well-known QFT algorithm, that runs in only $ O(\log n) $.

Oh, you wanted your output to be expressed as a usual vector, and it’s inconvenient for you to have its components registered in the quantum phases of a wavefunction? Well, no problem! There’s this method... _\*mumble\*_ phase estimation circuit... _\*mumble\*_ and that’s it, good luck!

</div>

<div style="flex: 0 0 48%; min-width: 300px; margin-bottom: 2em;" markdown="1">

**Bogo Fourier Transform (BFT)**<br>
For an input vector $ \mathbf{x} $:

1. Generate a random vector $ \mathbf{y} $.
2. Compute the inverse Fourier transform of $ \mathbf{y} $, denoted $ \text{FT}^{-1} [ \mathbf{y} ] $.
3. If $ \mathbf{x} = \text{FT}^{-1} [ \mathbf{y} ] $ return $ \mathbf{y} $, otherwise go back to step 1.

**Remark:** How do we compute the inverse Fourier transform on the second step? Ummm... there’s a MATLAB function that does that, right? That should do it.

</div>

</div>
