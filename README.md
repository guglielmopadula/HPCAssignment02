How to compile the code:
mpic++ -fopenmp -O3 kdtree.cc -o kdtree
How to run the code:
OMP_NUM_THREADS=6 mpirun -np 4 --map-by slot:PE=6 ./kdtree 2>/dev/null
