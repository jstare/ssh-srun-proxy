# ssh-srun-proxy

This is a small workaround to be able to use ssh/scp to node where you have running Slurm-jobs. It is not supposed to be a replacement to pam_slurm_adopt, but rather an alternative if you have a setup that isn't supported by pam_slurm_adopt.

## Installation

Place ````ssh-srun-proxy```` somewhere in the users ${PATH} and add content of ````ssh_config`````to /etc/ssh/ssh_config or ~/.ssh/config.

## Usage

Just run ssh as normal.

If you have more than one job running at the node you are trying to connect to you have to set SLURM_JOB_ID (or SLURM_JOBID).
