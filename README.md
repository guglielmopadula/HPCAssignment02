OMP_PROC_BIND=true OMP_PLACES=sockets OMP_NUM_THREADS=6 mpirun -np 4 --bind-to socket --map-by socket ./a.out 2>/dev/null | sort | uniq | wc -l

