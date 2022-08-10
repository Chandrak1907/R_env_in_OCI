OCI Data science environment primarily supports python. Below steps would create a conda environment with R in OCI data science environment

Steps:
1. Log into OCI data science notebook
2. Upload ***Renv.yaml*** file to /home/datascience
3. [Open a terminal](1.png)
4. Run ` odsc conda create -n Rname -f Renv.yaml --empty`  - This command will create a conda environment with Rnamev1_0
6. Run `conda activate /home/datascience/conda/Rnamev1_0` - Activates the above environment
7. Run `ipython kernel install --user --name=Rnamev1_0` -- Installs R kernel in jupyter notebook
8. Open jupyter notebook and select ***Rnamev1_0'*** and R kernel should be available
