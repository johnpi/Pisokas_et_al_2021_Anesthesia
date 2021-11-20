# Resources for the paper Pisokas et al. (2021) Anaesthesia Disrupts Distance, but not Direction, of Path Integration Memory. Current Biology. 

The most up to date version of this repository can be found at https://github.com/johnpi/Pisokas_et_al_2021_Anesthesia/


## Directory contents

Code/ : contain the source code used for data analysis and simulations.

Ant_Cooling_Data/ : contains the ant path recordings data.

Results/ : contains the processing results.



## Scripts

```Code/Simulation/path-integration-forget/collect_simulation_path_data.py```
The python script to use to run simulations and collect simulation data. Usage examples are shown inside the file. Data are stored in Code/Simulation/path-integration-forget/data/

```npz_to_csv.ipynb``` The script to convert the .npz files generated with the previous step to .csv files. 

```Code/analyse_trajectories.Rmd``` The R live script for calculating the trajectory statistics from the ant path recordings and the generated simulated paths. 

```Code/analyse_trajectories_publication.ipynb``` The python live script for recreating the plots used in the paper.  



## How to use

1. Run the script ```collect_simulation_path_data.py``` as shown in the examples listed in the comments to collect simulation data. To simplify usage I have included a pregenerated outbound trip recording (data/outbound_route_only_NW_to_SE_1500steps_03.npz) that the examples use. 

2. Follow the examples shown in ```collect_simulation_path_data.py``` to organise the generated files in directories. 

3. Use the script ```npz_to_csv.ipynb``` convert the .npz generated with the previous steps to .csv files. For that you would need to run ```jupyter notebook``` or ```jupyter lab``` and open this file in your web browser. 

4. Use the R live script ```Code/analyse_trajectories.Rmd``` for calculating the trajectory statistics from the ant path recordings and the generated simulated paths. To use this file you can open it in RStudio. 

5. Use the python script ```Code/analyse_trajectories_publication.ipynb``` for recreating the plots used in the paper. For that you would need to run ```jupyter notebook``` or ```jupyter lab``` and open this file in your web browser. 
