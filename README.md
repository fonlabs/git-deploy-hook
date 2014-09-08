How to use
==========

To use this, just copy&paste post-receive and deploy_config files in the hooks directory of the bare repo, 
giving execution permissions to the post-receive script. Also, get sure you have write permissions in the target
directory.

Example of usage:
```
% git init --bare ~/puppet
% cd puppet/hooks
% wget https://github.com/fonlabs/git-deploy-hook/archive/master.tar.gz -O - | tar --strip-components=1 -xzf -
% mv deploy_config ../
```