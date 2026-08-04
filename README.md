Several bash scripts that I have been iterating on to help automate some repetitive tasks encountered when building/running SENSEI

To use:

- clone this repo into your home directory
- add the following to your ```.bashrc``` (modify ```MY_WSL_USER_FOLDER``` and ```export MY_WINDOWS_USER_FOLDER``` to match your username):
```
export MY_WSL_USER_FOLDER="/home/<username>"
export MY_WINDOWS_USER_FOLDER="/mnt/c/Users/<username>"
if [ -f ~/BASH_SCRIPTS_FOR_SENSEI/.sensei_bash_functions ]; then
    . ~/BASH_SCRIPTS_FOR_SENSEI/.sensei_bash_functions
else
  echo "~/BASH_SCRIPTS_FOR_SENSEI/.sensei_bash_functions not found"
fi
```
- source your ```.bashrc``` (or close and re-open your terminal)

You should now have access to the following functions:
- ```cmake_debug```
- ```cmake_release```
- ```cmake_mpi_debug```
- ```cmake_mpi_release```
- ```cmake_vprt_debug```
- ```cmake_vprt-release```
- ```cmake_vprt_mpi_debug```
- ```cmake_vprt_mpi_release```
- ```SENSEI_HO_dev-debug```
- ```SENSEI_HO_dev-release```
- ```SENSEI_HO_dev-release_background```
- ```freeze_limiters```
- ```unfreeze_limiters```
- ```cfl_set_SENSEI```
- ```cfl_ramp_SENSEI```
- ```cfl_ser_SENSEI```
- ```cfl_expur_SENSEI```
- ```cfl_rdm_SENSEI```
- ```cfl_mrdm_SENSEI```
- ```clean_SENSEI```
- ```clean_restart_SENSEI```
- ```copy_nml_to_subfolders```
- ```run_SENSEI_cases```
- ```stop_SENSEI_cases```
- ```copy_SENSEI_results```


I'll try to update this with more utilities as needed, but feel free to modify these tools to your purposes. Remember to be careful though - these are simple bash functions and are far from foolproof.
