# TKHUD

This article provides executables of all frameworks and all datasets used in our research of Incremental Top-k High Utility Pattern Mining With Transaction Deletion.

The executables include all the frameworks, such as TKHUD, UMPD+K, HUIPRED+K, ITHUI+D, and PreTK+D and all the datasets which are used in our experiment: Retail, Mushroom, Chess, Chainstore, and T10I4D200K—T10I4D1000K.

All executables were compiled to run on 64-bit architectures.

Please refer to the following guide:

1. Note that the name of the executable for each algorithm is as follows:

| Original Name   | TKHUD | UMPD+K | HUIPRED+K  | ITHUI+D | PreTK+D | 
| --------------- | ----- | -----  | ---------- | ------- | ------- | 
| Executable Name | TKHUD | UMPD+K | HUIPRED+K  | ITHUI+D | PreTK+D |  

2. The parameters of the executables are as follows:

 for TKHUD, UMPD+K, HUIPRED+K, ITHUI+D, and PreTK+D
```bash
[0]          [1]       [2]                       [3]                           [4]                         [5]               [6]
[Executable] [K-value] [Utility Data Path(.txt)] [Transaction Data Path(.txt)] [Total Deletion Portion(%)] [Division Number] [Output File Name(.txt)]
```

3. Next, the characteristics of each dataset are as follows:

|  Dataset     | Number of Transactions| Number of Items | Average Transaction Length |
| ------------ | --------------------- | --------------- | -------------------------- |
| Retail       | 88,162                | 16,469          | 10.3                       |
| Mushroom     | 8,124                 | 119             | 23.0                       |
| Chess        | 3,196                 | 75              | 37.0                       |
| Chainstore   | 1,112,949             | 46,086          | 7.2                        |
| T10I4D200K   | 200,000               | 100             | 10.0                       |
| T10I4D400K   | 400,000               | 100             | 10.0                       |
| T10I4D600K   | 600,000               | 100             | 10.0                       |
| T10I4D800K   | 800,000               | 100             | 10.0                       |
| T10I4D1000K  | 1,000,000             | 100             | 10.0                       |

The datasets can be found at https://drive.google.com/file/d/1D_kgpaPYb-BrlFZM29T4PBMm-sZpLGcA/view?usp=sharing.

4. For example
```bash
TKHUD.exe 200 ../Data/utilRetail.txt ../Data/Retail.txt 2 4 TKHUD.txt 
```
will run TKHUD on Retail, with the k set to 200, the total deletion portion set to 2%, the division number set to 4, and the output file specified as TKHUD.txt.

5. The output directory "/out" is required for writing result patterns for all algorithms.

