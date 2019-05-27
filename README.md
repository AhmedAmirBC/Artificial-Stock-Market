# Artificial-Stock-Market

Modified Version of Artificial Stock Market to conform with research.

Based on the paper by [Hessay & Hadzikadik](http://computationalsocialscience.org/wp-content/uploads/2016/11/CSSSA_2016_paper_25.pdf).

# Changes made:


1. Fundamentalist investors are modelled as having a chartist component of their behavior. This is specified as a weight that is attached
to each type of behavior. Therefore, fundmentalists with a score of, say, 45, may attach a 50% weight to chartist behavior. In hindsight,
this probably does not make the model any more powerful.

2. Investors can place orders for up to 5 shares in a single period. This is done by repeatedly calling the market clearing function which
finds out stock supply and demand, and clears it out. There is probably a better mechanism to model large volume trades, but in the face of having more ambigious parameters, I stuck to the simplest solution.
