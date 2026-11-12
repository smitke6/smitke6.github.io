---
layout: post
category: joke
title: "Ineffective Fourier transforms"
date: 2017-05-30
---

*(A joke inspired by [xkcd #1185](https://xkcd.com/1185))*

<table style="width: 100%; border-collapse: collapse; text-align: left; border: none;">
  <tbody>
    <tr>
      <td style="width: 50%; padding: 0 20px 30px 0; vertical-align: top; border: none;" markdown="1">

**Lazy Fourier Transform (LFT)**<br>
For an input vector $ \bm{x} $:

1. Pad $ \bm{x} $ with zeros until its length is a power of 2.
2. Pad $ \bm{x} $ with more zeros until its length is a power of 3.
3. Give 'em a billion more zeros.
4. For a random prime $ p $, pad $ \bm{x} $ with more zeros until its length is a power of $ p $.
5. OK, now $ \bm{x} \equiv 0 $ approximately, hence its Fourier transform is the zero vector, so just return zero.

      </td>
      <td style="width: 50%; padding: 0 0 30px 20px; vertical-align: top; border: none;" markdown="1">

**Slow Fourier Transform (SFT)**<br>
For an input vector $ \bm{x} $:

1. Initialize $ \bm{y}=0 $.
2. Find a Gaussian fit for $ \bm{x} $.
3. The Fourier transform of a Gaussian is a Gaussian! Add the transformed Gaussian to $$ \bm{y} $$, and subtract the original Gaussian from $ \bm{x} $.
4. Repeat until $ \bm{x}=0 $, and then return $ \bm{y} $.

**Complexity:** I dunno, does it even converge?

      </td>
    </tr>
    <tr>
      <td style="width: 50%; padding: 0 20px 0 0; vertical-align: top; border: none;" markdown="1">

**Quantum Fourier Transform (QFT)**

1. Wait until they build a good enough quantum computer with a large number of qubits.
2. Run the well-known QFT algorithm, that runs in only $ O(\log n) $.

Oh, you wanted your output to be expressed as a usual vector, and it’s inconvenient for you to have its components registered in the quantum phases of a wavefunction? Well, no problem! There’s this method... _*mumble*_ phase estimation circuit... _*mumble*_ and that’s it, good luck!

      </td>
      <td style="width: 50%; padding: 0 0 0 20px; vertical-align: top; border: none;" markdown="1">

**Bogo Fourier Transform (BFT)**<br>
For an input vector $ \bm{x} $:

1. Generate a random vector $ \bm{y} $.
2. Compute the inverse Fourier transform of $ \bm{y} $, denoted $ \text{FT}^{-1} \left[ \bm{y} \right] $.
3. If $ \bm{x} = \text{FT}^{-1} \left[ \bm{y} \right] $ return $ \bm{y} $, otherwise go back to step 1.

**Remark:** How do we compute the inverse Fourier transform on the second step? Ummm... there’s a MATLAB function that does that, right? That should do it.

      </td>
    </tr>
  </tbody>
</table>
