# Kraken Metagenomics

The **Kraken Metagenomics** project aims to provide a solution for analyzing metagenomic data using the Kraken method. Metagenomics is a field of study that involves the analysis of genetic material recovered directly from environmental samples. It allows researchers to gain insights into the composition and function of microbial communities present in various ecosystems.

## Kraken Method

The Kraken method is a widely used tool for taxonomic classification of metagenomic sequences. It leverages a database of reference genomes to assign taxonomic labels to the input sequences based on sequence matches. The Kraken tool utilizes a k-mer-based approach to efficiently classify DNA sequences, making it suitable for analyzing large-scale metagenomic datasets.

## Dependencies

The project utilizes the following packages:

- `os`: Used for reading file addresses.
- `glob`: Enables reading file addresses.
- `gzip`: Allows reading zipped files.
- `pickle`: Used to store the index in memory.
- `pandas`: Facilitates reading information about bacteria.
- `ete3.NCBITaxa`: Used to read the tree of life of bacteria.
- `ncbi_genome_download`: Enables downloading bacterial genomes in zip format from NCBI.

## How to Run

To execute the project, follow these steps:

1. Open the `kraken.ipynb` file.
2. Upon execution, the script will first delete the existing tree of life.
3. Next, the bacterial genomes will be downloaded. If they have already been downloaded, this step will be skipped.
4. The index of the file will be created. If it has already been generated, this step can be skipped, and the index will be loaded from memory.
5. Provide the input and execute the algorithm on the reads.

## Construction of Metagenomics

To construct metagenomics data, follow these steps:

1. Open the `metagenomics-simulator.ipynb` file.
2. Execute the file to randomly select 10 bacteria.
3. Multiply the selected bacteria by the desired number of times and apply mutations.
4. Generate readings from the genomes similar to device-generated errors.
5. Save the generated data in the `metagenomic.txt` file.

## Contributions

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
