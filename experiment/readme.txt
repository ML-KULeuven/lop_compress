This file explains how to run the experiments.

First, install the necessary src files by running 'pip install .' in the main project folder.

Then, the different experiments can be run using the 'experiment/run.sh' bash script taking as input a settings file in the 'experiment/settings' folder.

You can create new settings files either manually or running the 'experiment/compression_experiment.py' file to automatically generate the settings based on some parameters.
For example: 'python3 compression_experiment list_compression_classification -m xgb | settings/xgb_classification.txt' saves the commands needed for the xgb binary classification experiment in settings/xgb_classification.txt.

Results will be saved in the 'experiment/results' folder and can be analysed using the tools in the 'experiment/icml.ipynb' notebook, which makes all the plots and tables for the paper.

Note: running experiment commands will create log files. If a log file exists and the experiment 'completed' then you would have to delete/rename the log file to run the experiment again. 
This is so that you can run partial experiments if it crashes.

The 'experiment/model_params.py' file can be adapted to change the range of parameters (for example for the scaling experiments).