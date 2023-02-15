# The Material Conditional

The material conditional for [Occam](https://occam.science).

The are two rules that effectively define the statement $P\to{Q}$ as being equivalent to $\neg(P\land\neg{Q})$. Specifically:

\[
\frac{\neg(P\land\neg{Q})}{P\to{Q}}\quad\small\text{[MaterialConditionalIntroduction]}
\]
\[
\frac{P\to{Q}}{\neg(P\land\neg{Q})}\quad\small\text{[MaterialConditionalElimination]}
\]

As well as these rules there are derived rules that rely on the above, plus rules from the [classical-propositional-logic](https://openmathematics.org/#classical-propositional-logic) and [de-morgans-laws](https://openmathematics.org/#de-morgans-laws) packages. They are:

\[
\frac{\neg{P}\lor{Q}}{P\to{Q}}\quad\small\text{[StrongerMaterialConditionalIntroduction]}
\]
\[
\frac{P\to{Q}}{\neg{P}\lor{Q}}\quad\small\text{[StrongerMaterialConditionalElimination]}
\]
&nbsp;
\[
\frac{P\Rightarrow{Q}}{P\to{Q}}\quad\small\text{[LogicalConsequenceInfersMaterialConditional]}
\]
\[
\frac{P\to{Q}}{P\Rightarrow{Q}}\quad\small\text{[MaterialConditionalInfersLogicalConsequence]}
\]
&nbsp;
\[
\frac{P\Rightarrow{R}\;\;Q\Rightarrow{R}\;\;P\lor{Q}}{R}\quad\small\text{[InferredDisjunctionElimination]}
\]

## Notes

To define the material conditional in anything other than a classical context is problematic, hence the dependency on the classical propositional logic package. 

The problem is that whilst $P\to{Q}$ is defined here as being equivalent to $\neg{P}\lor{Q}$, this is not the case in minimal or intuitionistic logic defined in the Hilbert style. 
In this style, just as for the logical connectives for disjunction $\lor$, conjunction $\land$ and falsum $\bot$, the logical connective for implication $\to$ is a primitive of the language and is not defined by way of an introduction rule, in fact it cannot be defined in terms of $\lor$, $\land$ and $\bot$ at all.

It could be argued that $\to$ defined here is not the same as $\to$ defined in Hilbert-style minimal and intuitionistic logics. 
Indeed, $\to$ in the Hilbert style is more akin to logical consequence $\Rightarrow$ in the natural deductive style. 
Such comparisons between variants of implication across logics are fraught, however, and are best avoided.

So why define the material conditional $\to$ here at all? 
Firstly, because the proofs of classical equivalence with logical consequence $\Rightarrow$ are illuminating, as are, it could be argued, the other proofs in this package. 
Secondly, although the divers and subtle meanings of implication are often disputed, not least amongst logicians, it seemingly does no harm to at least draw attention to two common variants here, and at least prove the commonly agreed upon classical equivalence between them.

## Contact

* https://djalbat.com
