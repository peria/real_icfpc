# ICFPC 2016
Details of the problem is written in [the official site](http://icfpc2016.blogspot.jp/).

# Abstract of my code
Finally, I automated to download problem information and to submit each solution.
These automated process was done with python scripts under [`bin/`](https://github.com/peria/real_icfpc/tree/master/2016/bin).
Simple explanation of the algorithm used in the solver is

- if the problem is a rotate-and-move
  - creates a mapping of 4 vertecies
- otherwise
  - wrap the destination object with two rectanles and chose the narrower one
    - each edge of the rectangle is parallel to xy-axis
    - each edge of the rectangle is almost 45 degree rotated to xy-axis

Solution program was written in C++, stored under [`src/`](https://github.com/peria/real_icfpc/tree/master/2016/src),
and [`problem.cc`](https://github.com/peria/real_icfpc/blob/master/2016/src/problem.cc) contains the main solver.

## directories
- bin : python scripts to run simple tasks automatically.
- html : visualizer written in a simple HTML and a JS file.
- problems : dumped files of problems.
- solutions : what I submitted in the contest.  Some solutions are invalid or exceeds size limit.
- src : source code and Makefile.  code is written in C++ and requires GMP library with C++ interface.


Note: this file was added after the contest.
