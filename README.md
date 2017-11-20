# resources.for.me

gatk discovering variants from rna-seq workflow
11/3/2017
https://software.broadinstitute.org/gatk/documentation/article.php?id=3891

list files on ftp server : curl -l ftp://ftp-trace.ncbi.nlm.nih.gov/sra/sra-instant/reads/ByStudy/sra/SRP/SRP041/SRP041179/

derr... cant download on compute node. So for downloading lots of sras just do this:

while read i; do fastq-dump $i; done < list.of.sras.

