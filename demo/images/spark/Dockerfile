ARG SPARK_VERSION=latest
FROM bitnami/spark:$SPARK_VERSION

USER root

RUN . /opt/bitnami/scripts/libcomponent.sh && component_unpack "python" "3.9.7-2" --checksum d102ab92a310673f8ec29bee5a3a93f1224db2680377742afbf383914f7abb1d

USER 1001

