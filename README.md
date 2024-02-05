# Genome Assembly using Illumina and Nanopore data

This project utilises both long-read (nanopore) data and short-read (illumina) data to conduct genome assembly. The pipeline conists of the quality control tool NanoPlot to assess the Nanopore reads. Also, the use of Minimap2 and Miniasm to align and assemble the reads, as well as the use of Bandage to visualise the assembled genome.

## Our Data
### The Short-Read Data:
Example name: *H3932_S4_L001_R1_001_fastqc.zip* and *H3932_S4_L001_R2_001_fastq.gz*

* H3932_S4 = Sample name
* L00* is the lane number i.e. 4 lanes were used
* R1 means it is a forward strand
* R2 means it is a reverse strand
* 001 = The file number
* .fastq.gz files are compressed FastQ files containing raw sequencing data
* fastqc.zip files are compressed archives containing the output files generated by FastQC

#### Our short-reads dataset contains 4 different reads, both with a forward and reverse strand 



### The Long-Read Data:
Example name: *FAQ09231_pass_barcode04_a6a5014a_0.fastq.gz* and fail one

* FAQ09231 = Sample name
* Pass = 
* Fail =
* Barcode is the
* a6a5014a is the
* 0 is the


## Figures
### NanoPlot Figure:

![NanoPlot KDE plot Example Image](https://github.com/mzywj2/Project-1---Group-4-Genome-Assembly/blob/main/newplot.png) 


The example plot above shows a plot comparing...

In addition to various plots, NanoPlot also creates a NanoPlot report which can be viewed by creating a web browser:

`python3 -m http.server 34567` - 34567 can be changed to your personalised 5 digit extension 

To view the report go to your web browser and type:

http://10.102.161.12:34567  - which is the ip and the hpc extension

### Miniasm Figure:

![Miniasm Image for a Short Read](https://github.com/mzywj2/Project-1---Group-4-Genome-Assembly/blob/main/SR%20Miniasm.png)

### Unicycler Figure

![Unicycler Image for a Short Read](https://github.com/mzywj2/Project-1---Group-4-Genome-Assembly/blob/main/SR%20Unicycler.png)



## Installation

### Nanoplot
Nanoplot can be installed using pip:

`pip install NanoPlot`

You may need to upgrade the pip version:

`pip install --upgrade pip`

For further detail about NanoPlot, refer to the NanoPlot GitHub Repository: https://github.com/wdecoster/NanoPlot.git

### Minimap2
Minimap can be installed using conda:

`conda install bioconda::minimap2`

For further detail about Minimap2, refer to the Minimap2 GitHub Repository: https://github.com/lh3/minimap2.git

### Unicycler
The most up to date version of Unicycler can be installed by:

`git clone https://github.com/rrwick/Unicycler.git`

`cd Unicycler`

`python3 setup.py install`

For further detail about Unicycler, refer to the Uncycler GitHub Repository: https://github.com/rrwick/Unicycler.git

### Bandage
Bandage can be installed using HomeBrew for OS or by downloading the binaries for other platforms, which can be found from the Bandage website (https://rrwick.github.io/Bandage/) or the Bandage GitHub Release Page (https://github.com/rrwick/Bandage/releases/). 

For installation on OS using HomeBrew:

`brew install bandage`

For further detail about Bandage, refer to the Bandage GitHub Repository: https://github.com/rrwick/Bandage.git


## Additional Resources
For more detailed explanations about each step of the process, refer to the following YouTube videos :

- [NanoPlot Tutorial] (https://www.youtube.com/watch?v=AeJj7_MMBTo): This video demonstrates how to use NanoPlot for quality control
- [Minimap2 Tutorial] (https://www.youtube.com/watch?v=f4sT5pEHoxU): This video explains the use of Minimap2 for mapping and Miniasm for genome assembly
- [Unicycler Tutorial] (https://www.youtube.com/watch?v=oTCLahU31Lg): This video demostrates the use of Unicycler for hybrid genome assembly
- [Bandage Tutorial]  (https://www.youtube.com/watch?v=avorVt8PxiY): This video shows how to install Bandage for Linux and usage for genome assembly visualisation 


## Contributions
If you found an issue or would like to submit an improvement to this project, please open an issue or submit a pull request.


## Acknowledgments
- Nanoplot: NanoPlot GitHub Repository: https://github.com/wdecoster/NanoPlot.git
- Minimap2: Minimap2 GitHub Repository: https://github.com/lh3/minimap2.git
- Unicycler: Unicycler GitHub Repository: https://github.com/rrwick/Unicycler.git
- Bandage : Bandage GitHub Repository: https://github.com/rrwick/Bandage.git and Bandage Website: https://rrwick.github.io/Bandage/
