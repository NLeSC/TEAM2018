# Sprint Name 

Bridging the gap

# Team leader

Dafne (only available the first 2,5 days of the sprint)

# Target project 

Bridging the gap

# Expertise required

Web services, APIs

# Size of team

4 or 5

# Description

In the Bridging the Gap project, we use [BlackLab](http://inl.github.io/BlackLab/) and the [corpus-frontend](http://acc.arabic-dh.hum.uu.nl/corpus-frontend) as a search engine for Arabic texts. In order to make the corpora easily searchable, the texts need to be processed by a morphological analyzer that extract _roots_ from the words. 

We created [cwl steps](https://github.com/arabic-digital-humanities/research-scripts/tree/master/adhtools/cwl) and combined them with nlppln into cwl workflows to process the text files and meta data with the morphological analyzers, and to index them for BlackLab. We currently manually run the workflows on a single VM on the HPC cloud. Then we transfer the resulting index files to a machine at the UU that runs an Apache webserver with BlackLab and corpus-frontend. 

It would be very useful if researchers can upload their own corpus to BlackLab. They should be able to upload a number of texts, and possibly a csv-file with metadata, which will be processed on the HPC cloud, and show up as corpora in BlackLab when they are done. The user defined corpora should only be available for the user that uploaded it.

# Goals
- Adjust CWL workflow so that it can handle metadata in csv (in preperation of sprint)
- Configure user management on the UU BlackLab server
- Make architectural design for communication between corpus-frontend, blacklab server and compute server
- Implement compute service on HPC cloud that runs a CWL workflow
- Implement upload client in BlackLab / corpus-frontend
