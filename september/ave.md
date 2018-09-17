# Allelic Variant Explorer demo

The Allelic Variation Explorer (AVE) is a web application to visualize (clustered) single-nucleotide variants across genomes.

There is a Docker image with the application and a sample dataset at https://github.com/nlesc-ave/ave-demo 

This Docker images is for showing the application works, to create a proper demo a scientific storyboard has to be written.

The story I have in mind is to take a gene which encodes for some trait (color, shape, stem size etc.) of a tomato and show that different tomato strains. Show the visual difference as pictures combined with the clustering of the genomes in the explorer.

This would require some literature searches and if the gene is not included in the sample dataset, a new dataset must be constructed.

A "text-book" example is tomato fruit color which is associated with several genes but one of the genes has a "major" effect, (Sl)MYB12 ([Adato et al., 2009](https://doi.org/10.1371/journal.pgen.1000777)). Many more gene-trait associations (or QTLs) for tomato have been obtained by mining literature (tables) (see the [candYgene](https://github.com/candYgene) project).
