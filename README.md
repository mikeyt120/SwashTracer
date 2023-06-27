# SwashTracer
Automated swash front tracing software for timestacks used in coastal research. Work detailed in Michael Thompson's PhD Thesis. 

# How to use
1. Open the SwashTracer_tool.ipynb in jupyter notebooks (I find anaconda distribution convenient).
2. Copy the Timestack_Shoreline_Xc_v0.model/ folder and your chosen timestack image file into your working directory. You can use the example_timestack.png which was created by Dr. Hannah Power. If you want to train and use a different model, use the SwashTracer_trainer.ipynb file.
3. The markdown text will guide you through the GUI for trimming your timestack and running the tracing algorithm.
4. Collect the traced timestack image and output data csv in the working directory.

# Content description
- SwashTracer_tool.ipynb - This tool allows the user to enter their own timestack image, set the user defined parameters using a GUI and run the automated swash tracing program to output swash front tracing data (csv file) and an annotated timestack.
- SwashTracer_trainer.ipynb - This trainer allows the user to train their own model and evaluate it according to the NRMSE metric described in the thesis.
- example_timestack.png - Full timestack image that can be used to try out the SwashTracer_tool.ipynb
- test_timestacks/ - This folder contains the timestack images and manually labelled point files for evaluating the NRMSE metrics described in the thesis.
- Timestack_Shoreline_Xc_v0.model/ - This folder contains the CNN model described in the thesis. It is the same model as v83 in the results google sheet.
- https://drive.google.com/drive/folders/10k3cSnvU_n3B2ee7BpJC8leSCIr-sS0b?usp=sharing - This google drive folder contains the training data. It is over 3 GB so not stored in the github repository.
- https://docs.google.com/spreadsheets/d/13iXW-CMyzlAxPTJHTx34q0H_k5yIES63VaTQNDhSgPM/edit?usp=sharing - This google sheet contains the training results of a lot of the earlier model versions with hyperparameter trial and error, as well as other results.

NOTE: The swash front tracing model v0 sometimes struggles to trace runup maximum and minimum regions. It is important that you visually check the traced timestack image for accuracy before using the results in the output data csv file.
