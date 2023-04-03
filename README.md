# Terminal Cheatsheet

### Logging in

ssh \<sunetid\>@login.sherlock.stanford.edu

### Edit files

`vi file.ext`

to edit `i`

when done, `esc` then `:x`


### Running .sh

`sbatch file.sh`

`squeue -u $USER`

`cat file.out`

### Feeding in outside variable values

in terminal:

`sbatch --export=N=1000,P_CONTROL=0.4,SAMPLE=1,DATASET=1,REPS=10 run_power.sh`

in file: 

`n_list= Sys.getenv('N')
p_list = Sys.getenv('P_CONTROL')
s_list = Sys.getenv('SAMPLE')
d_list = Sys.getenv('DATASET')
replications = Sys.getenv('REPS')`


torch is big to install, so use `pip install torch --no-cache-dir`


# Resources
[Sherlock Documentation](https://www.sherlock.stanford.edu/)

[Princeton Research Computing](https://researchcomputing.princeton.edu/support/knowledge-base/python)

[University of Florida Research Computing](https://help.rc.ufl.edu/doc/Using_Variables_in_SLURM_Jobs)

