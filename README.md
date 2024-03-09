[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/wM4-KOzy)
# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$


Proof:
If we use the same constants from the little-o definition in the big-O definition,
f(n) < c * g(n) for little-o, and
f(n) <= c * g(n) for big-O.
If f(n) < g(n) for all positive constants, then it must be true that f(n) is in big-O.
The difference of the two definitions is that little-o uses < which makes the growth much stricter when
compared to the definition for big-O. The definition for big-O uses a <= which makes the growth for g(x)
less restrictive. This difference between the definitions is the reason why little-o can imply big-O.

The other difference between the definitions is that the little-o definition requires the inequality to hold
for all positive constants while the big-o definition allows the inequality to hold for all $n \geq n_{0}$ and for the constant C. This makes it much less restrictive compared to the little-o definition.
