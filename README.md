# XMI-PRISM-Converter
UML diagrams as XMI files transformed to Discrete-Time Markov Chains (DTMCs) in PRISM language via the UnB-Dependability Analysis Library (UnB-DALi).

This project is to attempt to extract the information of an UML diagram in the form of an XMI file so that it can be used as input to the UnB-Dependability Analisys Library, that conducts the graph transformation of a UML diagram to a Discrete Time Markov Chain (DTMC) in the language of the PRISM model checker tool.

# How to use the XMI-PRISM-Converter tool

## Annotate the probabilities and Export the XMI file of your diagram

Follow the instructions for your tool inside the folder "docs/UML Modeling Tools Instructions".


## Run the JAR file via terminal
**Important: Make sure you have Java installed and added to your PATH environment variable.**

1) ** BUILD SOLUTION COMING SOON** Export the project as a runnable JAR file. Copy and paste this JAR file inside the folder where your XMI files are.
**Be sure that these files were generated by the same UML modeling tool.**

2) Go to this folder via terminal and enter a command according to what you want to do.
	
- If you want to convert all the XMI files inside the folder, run the command:
	
`java -jar xpconverter.jar`

- If you want to convert one or any arbitrary number of files, type their names as arguments, like:

`java -jar xpconverter.jar diagram1.xml diagram2.xml ... diagramN.xml`

3) Choose a number at the menu according to the modeling tool that generated the XMI files.

4) The result of the conversion(s) will show the file names alongside "[SUCCESS]" or "[FAIL]" messages.

For each **successfully** converted XMI file, an output, a PRISM file (.pm), will be created in the same folder, with the same name as the original file.
