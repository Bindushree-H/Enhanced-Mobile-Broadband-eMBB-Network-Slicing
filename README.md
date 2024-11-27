#Enhanced-Mobile-Broadband-eMBB-Network-Slicing

INTRODUCTION

This project aims to provide a framework to develop and evaluate network slicing techniques for Wi-Fi networks. We provide a customizable Wi-Fi indoor scenario, realized with the ns-3 network simulator (version ns-3.30), in which several mobile Stations (STAs) are connected to an Access Point (AP) placed in the centre of a room. In general, the STAs have distinct performance requirements, and are grouped in different networks slices (e.g. eMBB, mMTC and URLLC).

On top of this scenario, we facilitate the implementation and the testing of radio resources allocation algorithms to realize network slicing in the radio access segment of Wi-Fi networks. In particular, three steps need to be followed as,Configure the environment parameters, such as the number of Wi-Fi STAs, required throughput in each slice and the dimensions of the room.

Write a dynamic algorithm which allocates radio resources at each time slot, by receiving in input the run-time Key Performance Indicators (KPIs) of the network. There is no limit on the kind of algorithm which can be implemented, and also Machine Learning (ML) techniques are supported.
Finally, when the simulation time is over, the experienced performance (i.e. throughput, error probability, latency, energy consumption and spectrum efficiency) can be accessed from a .csv file.


EXECUTION

We can find detailed instructions on how to use our framework to validate your network slicing algorithms through simulations in ns-3. First of all, execute the following steps to be able to use our codes:
•	Install the ns-3 network simulator in your machine following the instructions from the main website nsnam.org
•	Download this repository as a .zip and extract it.
•	Paste its content inside the scratch directory, which is inside the ns-3 release directory, automatically created upon the ns-3 installation.
Configure Simulation Parameters:
•	The project allows customization of simulation parameters, such as the number of stations, transmission power, simulation time, frequency band (e.g., AX_5), and more. These parameters will be used for running the simulation to model how 5G network slicing works within a Wi-Fi network.
•	The repository likely provides configuration or script files for the simulation setup. Review the README or script files to ensure you adjust parameters like the number of stations, channels, or simulation duration according to your needs.
Run Simulation:
•	After adjusting the parameters, run the simulation by invoking the corresponding NS3 script. This might look like:
./waf --run <simulation_script_name>
•	The simulation will execute based on the provided parameters.
Result Generation:
•	 During the execution, monitor the terminal for progress updates or errors. Ensure that there are no dependency issues or missing configuration files.
•	Once the simulation completes, the output is typically written to a CSV or log file, detailing metrics such as throughput, latency, or the performance of the network slices under different conditions.
Executing this repository involves understanding the network simulation process in NS3, modifying simulation configurations, running the script, and analyzing the results for insights related to 5G network slicing and its application to Wi-Fi networks. Always refer to the repository’s documentation for specific steps and parameters.


RESULT


The results of the "5g-network-slicing-for-wifi-networks" repository reveal valuable insights into the performance of Wi-Fi networks when integrated with 5G network slicing. Through simulations, the repository demonstrates how different configurations of network slices can significantly influence the overall efficiency of the Wi-Fi network. By varying parameters like bandwidth, the number of stations, and slice configurations, the tool generates data that highlights improvements in throughput, latency, and resource allocation. The results also underscore the potential of 5G slicing to optimize Wi-Fi performance, particularly in high-demand scenarios, showcasing the flexibility and scalability that can be achieved through network slicing. 

OUTPUT

Test file's are created
