FROM apache/spark:4.0.0

ENV DELTA_VERSION=4.0.0 \
    HADOOP_VERSION=3.4.1 \
    SCALA_VERSION=2.13

RUN mkdir -p /opt/spark/jars

ADD https://repo1.maven.org/maven2/io/delta/delta-spark_${SCALA_VERSION}/${DELTA_VERSION}/delta-spark_${SCALA_VERSION}-${DELTA_VERSION}.jar \
    /opt/spark/jars/
ADD https://repo1.maven.org/maven2/org/apache/hadoop/hadoop-aws/${HADOOP_VERSION}/hadoop-aws-${HADOOP_VERSION}.jar \
    /opt/spark/jars/
ADD https://repo1.maven.org/maven2/software/amazon/awssdk/bundle/2.31.78/bundle-2.31.78.jar \
    /opt/spark/jars/