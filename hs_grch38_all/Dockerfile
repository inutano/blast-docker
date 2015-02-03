FROM inutano/blast-docker

WORKDIR /data
RUN wget ftp://ftp.ensembl.org/pub/current_fasta/homo_sapiens/cdna/Homo_sapiens.GRCh38.cdna.all.fa.gz && \
    gunzip -f Homo_sapiens.GRCh38.cdna.all.fa.gz && \
    makeblastdb -in Homo_sapiens.GRCh38.cdna.all.fa -dbtype nucl -hash_index

CMD ["bash"]
