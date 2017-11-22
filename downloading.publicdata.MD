for i in {493..536}; do echo ftp://ftp-trace.ncbi.nlm.nih.gov/sra/sra-instant/reads/ByStudy/sra/SRP/SRP041/SRP041179/SRR1238$i/SRR1238$i.sra; done
so for i in series then get series that way replace echo with wget

for getting the fastq simply
curl https://www.ebi.ac.uk/arrayexpress/files/E-GEOD-56796/E-GEOD-56796.sdrf.txt | cut -f33 > fastqslist
sed -i '1d' fastqs
while read i; do wget $i;done < fastqs
