# Genome Assembly using Illumina and Nanopore data

This project utilises both long-read (nanopore) data and short-read (illumina) data to conduct genome assembly. The pipeline conists of the quality control tool NanoPlot to assess the Nanopore reads. Also, the use of Minimap2 and Miniasm to align and assemble the reads, as well as the use of Bandage to visualise the assembled genome.

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

### Bandage
Bandage can be installed using HomeBrew for OS or by downloading the binaries for other platforms, which can be found from the Bandage website (https://rrwick.github.io/Bandage/) or the Bandage GitHub Release Page (https://github.com/rrwick/Bandage/releases/). 

For installation on OS using HomeBrew:

`brew install bandage`

For further detail about Bandage, refer to the Bandage GitHub Repository: https://github.com/rrwick/Bandage.git


## Additional Resources
For more detailed explanations about each step of the process, refer to the following YouTube videos :

- [NanoPlot Tutorial] (): This video
- [Minimap2 Tutorial] (): This video
- [Bandage Tutorial]  (): This video


## Acknowledgments

