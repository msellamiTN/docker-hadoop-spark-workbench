FROM bde2020/hadoop-namenode:1.1.0-hadoop2.8-java8
MAINTAINER Sellami Mokhtar<mokhtar.sellamit@data2-ai.com>

LABEL description="Install pig on hadoop 2.8 image."

ENV PIG_VERSION 0.17.0

RUN wget -q http://apache.osuosl.org/pig/pig-$PIG_VERSION/pig-$PIG_VERSION.tar.gz && \
   tar xzf pig-$PIG_VERSION.tar.gz -C /usr/local/  && \
   ln -s /usr/local/pig-$PIG_VERSION /usr/local/pig  && \
   rm pig-$PIG_VERSION.tar.gz

ENV PATH $PATH:/usr/local/pig/bin
ENV HADOOP_MAPRED_HOME /usr/lib/hadoop-mapreduce
