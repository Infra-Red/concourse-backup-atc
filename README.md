# concourse-backup-atc

Configure Concourse ATC backups in a Concourse pipeline.

## Prerequisites

1. [Git](https://git-scm.com)
1. [Concourse](http://concourse.ci)

## Steps to use this pipeline

```bash
git clone https://github.com/Infra-Red/concourse-backup-atc 
cp secret{.example,}.yml
vim secret.yml 
fly -t $CONCOURSE_TARGET set-pipeline --pipeline backup-atc --config ci/pipeline.yml -l secret.yml
```
