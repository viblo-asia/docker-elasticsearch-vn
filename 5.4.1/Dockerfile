FROM docker.elastic.co/elasticsearch/elasticsearch:5.4.1

ARG extension=https://github.com/duydo/elasticsearch-analysis-vietnamese/releases/download/v5.4.1/elasticsearch-analysis-vietnamese-5.4.1.zip

RUN cd /usr/share/elasticsearch \
    && bin/elasticsearch-plugin install analysis-icu \
    && bin/elasticsearch-plugin install analysis-kuromoji \
    && bin/elasticsearch-plugin install $extension
