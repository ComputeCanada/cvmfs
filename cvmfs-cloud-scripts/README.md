

There are different approaches to enable CVMFS on a cloud, either by adding a Customization Script when launching a VM, or install & configure directly on a running VM, or even apply it to your own cloud image(s). 

* Here is the script for different OS flavors:

  -- For CentOS/Redhat: ![CVMFS Customization Script](https://github.com/ComputeCanada/CVMFS/blob/main/cvmfs-cloud-scripts/customization_script_CtosRH)

  -- For Fedora: (TBD) 

  -- For Ubuntu/Debian:(TBD) 

  -- For SLES/OpenSUSE: (TBD) 

  -- For Windows: (TBD) 


* To enable CVMFS via Openstack Dashboard:

![Alt Install_CVMFS_on_your_VM](https://user-images.githubusercontent.com/73720293/97760381-a80ae600-1ac8-11eb-904f-5861c93d6bd8.png)

* To enable it on a running VM

Just run the script on your VM, it will perform all the setup steps for you.  

* Once it's installed and configured, you can test CVMFS by running:

```
$ ls /cvmfs/soft.computecanada.ca
config  custom  easybuild  gentoo  new_repository  nix
```

or list any other repositories you added to CVMFS_REPOSITORIES variable. 


* Now, you can run the following command to enable software modules from CVMFS:

`$ source /cvmfs/soft.computecanada.ca/config/profile/bash.sh`

* More details please refer to: https://docs.computecanada.ca/wiki/Accessing_CVMFS





