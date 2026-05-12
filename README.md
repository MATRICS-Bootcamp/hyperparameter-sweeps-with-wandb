# Running Hyperparameter Sweeps with Weights & Biases on Distributed Systems

In this tutorial, you'll learn:

* Multiple ways to interact with a container from the command line
* How to automate a hyperparameter sweep with Weights & Biases (W&B) and Slurm arrays
* How to track these runs using the W&B dashboard and Slurm commands


Setting up a W&B sweep on an HPC cluster

Authenticating W&B inside an Apptainer container
Defining a hyperparameter search space in sweep.yaml
Launching parallel sweep agents with Slurm job arrays


Monitoring and retrieving results

Tracking runs in the W&B dashboard
Retrieving the best configuration via the W&B API


## Today's Tutorial Agenda

* Authenticating Weights & Biases on Sherlock or Farmshare [[link](running-wandb-on-hpc.md#step-1-authenticating-your-weights--biases-account-from-sherlock-or-farmshare)]
* Setting up your training script [[link](running-wandb-on-hpc.md#step-2-set-up-your-training-script)]
* Defining your sweep configuration [[link](running-wandb-on-hpc.md#step-2-define-the-sweep-configuration)]
* Writing an Sbatch script to run your sweept [[link](running-wandb-on-hpc.md#step-3-write-an-sbatch-script-to-run-your-sweep)]
* Using `array` to launch parallel `wandb` sweep agents [[link](running-wandb-on-hpc.md#step-4-use-array-in-sbatch-to-launch-perfectly-parallel-wandb-agents)]
* Monitoring your sweep on the W&B dashboard [[link](running-wandb-on-hpc.md#step-5-monitor-your-sweep-on-the-wb-dashboard)]
* Retrieve the best sweep configuration [[link](running-wandb-on-hpc.md#step-6-retrieve-the-best-configuration-directly-on-sherlock)]

### Do you have any questions? 
Please reach out to us at [matrics-bootcamp@stanford.edu](mailto:matrics-bootcamp@stanford.edu) or set up a General Consultation with us at [this link](http://sdss-compute-consultation.stanford.edu/).

### Would you like to provide feedback?
Please provide anonymous feedback [here](https://forms.gle/x3wB8qMPWBbeNosR9).