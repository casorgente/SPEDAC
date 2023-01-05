# SPEDAC

This repository hosts the collection of instances used in the computational study conducted in the paper _"Shortest Paths with Exclusive-Disjunction Arc Pairs Conflicts"_ by R. Cerulli, F. Guerriero, E. Scalzo and C. Sorgente.

The RAND and NWS folders contain 540 random and 135 small-world topology network instances, respectively.

Each file contains, on the first line, a summary of the instance characteristics, including:
- the number of nodes (<code>n</code>);
- the number of arcs (<code>m</code>);
- the arc density (<code>density</code>);
- the conflict density (<code>conf_density</code>);
- the range of arc costs (\[<code>elb</code>,<code>eub</code>\]);
- the range of conflict penalties (\[<code>clb</code>,<code>cub</code>\]);
- the random seed used to initialize the random number generator (<code>seed</code>).

The second line, starting with <code>p</code>, reports the number of nodes, number of arcs and number of conflicts of the instance.

The subsequent two lines, starting with <code>s</code> and <code>t</code> indicate the source and target vertices, respectively.

The remaining lines start with <code>a</code> or <code>c</code>. 
In the former case, the line represents an arc _(u,v)_, in the format <code>u v _cost_</code>.
In the latter case, the line represents a conflict between two arcs, let say _(u,v)_ and _(w,z)_, in the format <code>u v w z _penalty_</code>.