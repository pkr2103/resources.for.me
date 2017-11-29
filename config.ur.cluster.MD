
download miniconda to random location: wget + linux installation
download sratoolking: wget + https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/current/sratoolkit.current-ubuntu64.tar.gz
add the bin folder of sratoolkit to preappend bashrc path with export PATH="blah.blah:sratoolkit/bin:$PATH"

submitting job with java. need to specify memory twice (potentially)#

in script /path/to/java -XmxMEM...AMOUNT...IN...MB
in submission command qsub -l h_vmem=15G (or can do it in script with #$ -l h_vmem=15G or amount you want
