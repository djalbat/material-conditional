# The Material Conditional

The material conditional for the [Occam](http://djalbat.com/occam) proof assistant.

The are two rules that effectively define the statement $P\to{Q}$ as being equivalent to $\neg(P\land\neg{Q})$. Specifically:

\[
\frac{\neg(P\land\neg{Q})}{P\to{Q}}\quad\small\text{[MaterialConditionalIntroduction]}
\]
\[
\frac{P\to{Q}}{\neg(P\land\neg{Q})}\quad\small\text{[MaterialConditionalElimination]}
\]

## Contact

* jecs@imperial.ac.uk
* http://djalbat.com
