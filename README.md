# SwashTracer
Automated swash front tracing software for timestacks used in coastal research.

# How to use
1. Open the SwashTracer_CNN.ipynb in jupyter notebooks (I find anaconda distribution convenient).
2. Copy the michaelThompson_imgSize_64.model file and your chosen timestack file into your working directory. You can use the example_timestack.png which was created by Associate Professor Hannah Power. If you want to train and use a different model, see this github repo https://github.com/mikeyt120/swash_zone_tracing_SAI2020.
3. Run each cell in the SwashTracer_CNN.ipynb file. The markdown text will guide you through the GUI for trimming your timestack and running the tracing algorithm.
4. Collect the traced timestack image and output data csv in the working directory.
