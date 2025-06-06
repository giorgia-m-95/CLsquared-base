# CLsquared: a Cleaning and Clustering tool for viral genome analysis

CLsquared is a command-line pipeline designed to identify and retain high-quality viral sequences from both public and private datasets. It flags sequences with unconfirmed mutation patterns as potentially incorrect, ensuring more reliable downstream analyses. Every filtering step in the pipeline is fully customizable, allowing users to fine-tune the process to their specific requirements.

CLsquared is effective for processing large-scale datasets, such as GISAID or NCBI SARS-CoV-2 and Monkeypox repositories. 

The CLsquared-base pipeline exploits the Python *polars* library to optimize computational efficiency. 
Large FASTA files can be split into smaller chunks, which are processed sequentially further contributing to reduced computational time.

A detailed description of each cleaning step can be found at //, in the header of each script, or by using the --help command with each script.

A <code style="color: blue">Docker</code> version of the pipeline can be foun at //

### Install

The CLsquared pipeline can be installed through the following command:
<code style="color: cyan">git clone https://github.com/giorgia-m-95/CLsquared-multiprocessing/</code>

### Dependencies

CLsquared requires Python 3 (https://www.python.org/) and the installation of the following python packages:

- pip3 install biopython v. 1.81
- pip3 install jenkspy v. 0.4.1
- pip3 install kneebow v. 1.0.2
- pip3 install multiprocessing
- pip3 install numpy v. 1.25.1
- pip3 install pandas v. 2.0.3
- pip3 install polars v. 1.21.0
- pip3 install plotly v. 5.17.0
- pip3 install statistics

### References

- [Polars](https://pola.rs/)
- Heng Li, Bob Handsaker, Alec Wysoker, Tim Fennell, Jue Ruan, Nils Homer, Gabor Marth, Goncalo Abecasis, Richard Durbin, 1000 Genome Project Data Processing Subgroup, The Sequence Alignment/Map format and SAMtools, Bioinformatics, Volume 25, Issue 16, August 2009, Pages 2078–2079, https://doi.org/10.1093/bioinformatics/btp352
- Shu, Y., & McCauley, J. (2017). GISAID: Global initiative on sharing all influenza data - from vision to reality. Euro surveillance : bulletin Europeen sur les maladies transmissibles = European communicable disease bulletin, 22(13), 30494. https://doi.org/10.2807/1560-7917.ES.2017.22.13.30494
- O’Leary NA, Cox E, Holmes JB, Anderson WR, Falk R, Hem V, Tsuchiya MTN, Schuler GD, Zhang X, Torcivia J, Ketter A, Breen L, Cothran J, Bajwa H, Tinne J, Meric PA, Hlavina W, Schneider VA. Exploring and retrieving sequence and metadata for species across the tree of life with NCBI Datasets. Sci Data. 2024 Jul 5;11(1):732. doi: 10.1038/s41597-024-03571-y. PMID: 38969627; PMCID: PMC11226681.
- James Hadfield, Colin Megill, Sidney M Bell, John Huddleston, Barney Potter, Charlton Callender, Pavel Sagulenko, Trevor Bedford, Richard A Neher, Nextstrain: real-time tracking of pathogen evolution, Bioinformatics, Volume 34, Issue 23, December 2018, Pages 4121–4123, https://doi.org/10.1093/bioinformatics/bty407
