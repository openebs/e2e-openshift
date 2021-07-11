# e2e-konvoy
This repository contains platform execution code to run OpenEBS and workloads E2E testing pipelines on D2IQ-Konvoy platform. The platform is built around GitLab and OpenEBS Litmus.

## Pipeline stages

Each of the pipelines has the following five stages

1. Konvoy cluster setup
2. OpenEBS setup
3. Functional tests
4. Chaos tests
5. Cleanup

## How it works?

`master` branch contains the test description and the procedure to execute the tests. `OpenEBS-Base`pipeline includes the test scripts which validates OpenEBS storage by triggering litmus experiments. It also validates the functionality of OpenEBS components.