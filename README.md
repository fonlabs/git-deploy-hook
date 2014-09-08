How to use
==========

To use this, just copy&paste post-receive and deploy_config files in the hooks directory of the bare repo, 
giving execution permissions to the post-receive script. Also, get sure you have write permissions in the target
directory.

Example of usage:
```
# '%' denotes remote ssh session
# '$' denotes local session
$ ssh -oForwardAgent=yes machine
% git init --bare ~/puppet
% cd puppet/hooks
% git archive --remote=https://github.com/fonlabs/git-deploy-hook.git master | tar xf - 
```