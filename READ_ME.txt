HOW TO RUN
after downloading the code, we need to import gurobipy using the cmd "!pip install gurobipy==10.0.1".
the function we need to run is solve_project(file_path), this function takes a .txt file with the problem in it in the following format:
##
MAX/MIN f(x,y,z,...)
VAR x y z ...

Subject To
c1 g(x,y,z,...) >= 0
c2 ...
...
#
f being the objective function, then the Variables and last the constraint g ( constraint line should start with cN - N being constraint number ).
 SEE problem_1 for example.

Then change the intial point in solve_project(file_path) function to wanted point to local varible "prev_point", and also add random point to "new_point".
then RUN the python function solve_project(file_path)
