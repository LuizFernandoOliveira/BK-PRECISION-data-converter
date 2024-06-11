# SIGLENT-data-converter
Data Converter for SIGLENT SDG1032X Arbitrary Function Generator

Basic example is a simple sine wave;
- Files can have up to 16384 data values;
- Format is header than a list of voltaqge point in vertical list without the time coordinate;
- Volts can be fix or sci notation.

Header must be in form:

![image](https://github.com/LuizFernandoOliveira/SIGLENT-data-converter/assets/50978651/57d686a0-f9eb-4419-9f07-5b33065706e8)

At least one empty line at the end of file.

- The maximum rate of output of the table is 30 MHz;
- File can be .txt or .csv;
- Param in the header are read to initialise the generator;
- Frequency must be consistent;
- Amp is the expected pk-pk amplitude;
  
# How to run

Run the "main.m" file in MATLAB R2023b. After executing the code, MATLAB will generate the "output.csv" file in the same folder as the "main.m" file. This file "output.csv" represents the signal generated in MATLAB in CSV format with the header recognized by the SIGLENT SDG1032X Arbitrary Function Generator.

# Example

Signal generated in MATLAB:

![fig](https://github.com/LuizFernandoOliveira/SIGLENT-data-converter/assets/50978651/1c87e61a-50e2-4154-81d6-3643ac74de4a)

Signal reproduced on the RIGOL Oscilloscope:

![RigolDS0](https://github.com/LuizFernandoOliveira/RIGOL-data-converter/assets/50978651/d01e4d85-7ada-48d1-a17a-ad654770aef1)

