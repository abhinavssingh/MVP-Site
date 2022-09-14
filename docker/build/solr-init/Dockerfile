# escape=`

ARG BASE_IMAGE
ARG SXA_IMAGE

FROM ${BASE_IMAGE}
FROM ${SXA_IMAGE} as sxa

SHELL ["powershell", "-Command", "$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]

COPY --from=sxa C:\module\solr\cores-sxa.json C:\data\cores-sxa.json