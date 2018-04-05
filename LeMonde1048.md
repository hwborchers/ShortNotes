
# Le Monde Puzzle #1048

The Le Monde Puzzle #1048 from April 1, 2018, says:

> A magical integer m is such that the remainder of the division 
> of any prime number p by m is either a prime number or 1. What 
> is the unique magical integer between 25 and 100? And is there 
> any less than 25?

It is quite easy to actually prove by hand that 4,6,8,12,18,24,30 are the only magical numbers up to 30. That there are no more magical numbers follows from Dirichlet's theorem and the fact, if $p_1, p_2, ..., p_n$ are the first n primes, that 
$p_{n+1}^2 < p_1 \cdot ... \cdot p_n$ for $n \ge 4$ !

The first remark is that the problem reduces to look at the *rest classes* modulo a number $m$, i.e., $m$ is 'magical' if for all primes $p$ the rest class $\mod(p, m)$ is 1 or a prime. $m$ itself cannot be prime because $\mod(p, p) = 0$.

Remember that there are always (infinitely many) primes in an *arithmetic progression* $\{a \cdot m + r | \, a = 0, 1, 2, ...\}$ if $m$ and $r$ are coprime. For $m$ to be non-'magical' there must be a rest class $r$ such that $r$ is not 1, not a prime, and coprime to $m$.

The first composite number would be 4, but its rest classes are $0, 1, 2, 3$ and thus $\mod(p, 4)$ is 1 or prime. This continues for $m = 6$ $m = 8$, the next interesting case being $m = 10$. Here $r = 9$ fulfills the conditions and 10 is not 'magical'. The same kind of argument applies to all numbers up to 30 resulting in 4,6,8,12,18,24,30 being 'magical'.

Looking at the possible rest classes $0, 1, 2, 3, 4, 5, ...$ for larger $m$, it becomes clear that $m$ must be divisible by 2, 3, and 5 at least to prevent the remainders 4, 9, and 25 to come into the way with non-primes in their rest classes. $m = 60$ is prevented by 49, the next possible 'magical' number can only be $m = 210 = 2 \cdot 3 \cdot 5 \cdot 7$, prevented by $11^2 = 121 < 210$.

This argument again continues: If $m = p_1 \cdot ... \cdot p_n$, where $p_1, ..., p_n$ are the first $n$ primes, then $p_{n+1}^2$ is a rest class that is non-prime and coprime to $m$. And it is smaller than $m$ because $p_{n+1}^2 < p_1 \cdot ... \cdot p_n$ for all $n \ge 4$. This concludes to show that there are no more 'magical' numbers.

(Note: The last inequality follows from Bertrand's Postulate:

(1) $p_{n+1}< 2 p_n$  
(2) $p_{n+1}^2 < 4 p_n^2 < 8 p_n p_{n-1}$  
(3) $p_{n+1}^2 < p_1 p_2 p_3 ... p_{n-1} p_n$

for $n \ge 5$ (and for $n = 4$ by direct verification, see $p_5 = 11$).

Reference: https://xianblog.wordpress.com/2018/04/01/le-monde-puzzle-1047/
