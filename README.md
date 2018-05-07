# The Material Conditional

The material conditional for the [Occam](http://djalbat.com/occam) proof assistant.

The are two rules that effectively define the statement $P\to{Q}$ as being equivalent to $\neg(P\land\neg{Q})$. Specifically:

\[
\frac{\neg(P\land\neg{Q})}{P\to{Q}}\quad\small\text{[MaterialConditionalIntroduction]}
\]
\[
\frac{P\to{Q}}{\neg(P\land\neg{Q})}\quad\small\text{[MaterialConditionalElimination]}
\]

As well as these rules there are derived rules that rely on the above, plus rules from the [propositional logic](https://openmathematics.org/#propositional-logic) and [de-morgans-laws](https://openmathematics.org/#de-morgans-laws) packages. They are:

\[
\frac{\neg{P}\lor{Q}}{P\to{Q}}\quad\small\text{[StrongerMaterialConditionalIntroduction]}
\]
\[
\frac{\neg{P}\lor{Q}}{P\to{Q}}\quad\small\text{[StrongerMaterialConditionalElimination]}
\]
&nbsp;
\[
\frac{P\Rightarrow{Q}}{P\to{Q}}\quad\small\text{[LogicalConsequenceInfersMaterialConditional]}
\]
\[
\frac{P\to{Q}}{P\Rightarrow{Q}}\quad\small\text{[MaterialConditionalInfersLogicalConsequence]}
\]
\[
\frac{P\Rightarrow{R}\;\;Q\Rightarrow{R}\;\;P\lor{Q}}{R}\quad\small\text{[InferredDisjunctionElimination]}
\]

## Contact

* jecs@imperial.ac.uk
* http://djalbat.com
