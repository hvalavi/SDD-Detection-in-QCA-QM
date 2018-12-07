# QM Stray-Charge Defect Analyzer
Applicaion was developed under .Net Framework +4.0 for MS Windows Platform
# Prerequisite:
	0. MS Windows
	1. MS .Net Framework ver 4.0 or higher
	2. 'maj' File must exist in the same directory as application executable file is located
# How to use:
	0. Run the executable file (QCA_Just_StrayCharge.exe)
	1. Specify the movement distance of Stray-Charge on each iteration both for X and Y axes. Default step is 0.1nm per itteration (The program then moves the Stray Charge in a rectangle of size 13.1x16.1 nm, the center of this rectangle is the QM central cell).
	2. Program needs some pre-defined directories just beside it's executable file. First generate them by pressing "F" key on keyboard.
	3. Then you can generate circuits using G command (simply press G on your keyboard). Generated files must be found at "Output" directory. List of the generated files was also created at the "Dictionary.txt" file.
	4. Simulation Time can be pridected using P command. Specify simulation time of each circuit on your computer and number of cpu cores your machine can supply for simulation. It then returns simulation time and output size.
	5. Simulation can be done using W command. Specify required parameters or leave them for Default values.
		note1: do not use your computer while simulating. Any intterupt may lead automatic-simulation to fail!
		note2: set Time paramter according to your system abilities. A good approximation is to time one simulation of 'maj' file manualy using QCADesigner.
		note3: Enter number of cores in range 1 (Program'll use the single core on the system) to maximum logical cores you have installed on your system.
		note4: For single core systems (old ones), 0 must be entered instead of above range.
		note5: Simulation results was stored in "Results" directory.
	6. After Simulation, you can analyze the results using "A" command.
		note: "Analyze.txt" file structure is like below:
			Y_axis_iteration$X_axis_iteration$point_of_transition
note: The Other options/commands have specific objectives:

	Split : Split Simulation files to some partions to run on different machines.

	Clean Inputs : Delete all circuits in "Results" directory that have been failed to simulate.
# Results
The full simulation results are available in "final.zip" file.
note: "final.zip" has 7 other parts ("final.z01" to "final.z07") that are required.
note: these results were generated under default parameters.






