# Community Software Analysis Written Report

## Software: *Dask*

Dask is a software package that extends popular data libraries in Python such as numpy, pandas, and scikit-learn to allow scalable parallel computation. Dask uses dynamic task scheduling to allow execution on these extended data collections in distributed environments. This means that tasks are scheduled according to a task graph dynamically created by the scheduler as requests for computation arrive.

### Stats

| Description | Your answer |
|---------|-----------|
| Repository URL | https://github.com/dask/dask |
| Main/documentation website | https://docs.dask.org/ |
| Year project was started | 2015 |
| Number of contributors in the past year | 150 |
| Number of contributors in the lifetime of the project | 341 |
| Number of distinct affiliations | 5-10 |
| Where do development discussions take place? | https://gitter.im/dask/dev, Github, monthly meeting |
| Typical number of emails/comments per week? | 5 github issues |
| Typical number of commits per week? | 10-20 commits |
| Typical commit size | 1-5 files changed, some changes much larger |
| How does the project accept contributions? | yes |
| Does the project have an automated test suite? | yes |
| Does the project use continuous integration? | yes |
| Are any legal/licensing steps required to contribute? | no |

Key developers:

* Matthew Rocklin @mrocklin (NVIDIA)
* Martin Durant @martindurant (Anaconda)
* Tom Augspurger @TomAugspurger (Anaconda)
* Jim Crist-Harif @jcrist (Anaconda)
* Antoine Pitrou @pitrou (Anaconda)
* James Bourbeau @jrbourbeau (Quansight)
* Olivier Grisel @ogrisel (Inria)
* Stephan Hoyer @shoyer (Google)
* John Kirkham @jakirkham (HHMI/Janelia)

### Funding

Dask is funded by NumFOCUS (https://numfocus.org). NumFOCUS promotes open source software in scientific computing by sponsoring projects like dask and through educational programs like PyData. Some dask contributors are paid by corporations to work mainly on dask.

### Purpose and Key Stakeholders

The purpose of dask is to allow scientific python to scale to clusters, but also get the most out of workstations and laptops. Dask implements familiar APIs (e.g. from numpy, scipy, xarray, and scikit-learn), and provides monitoring and exception handling.

Organizations using dask:
1. Pangeo
    1. Open-source platform for high-performance geoscience
    2. Uses dask-kubernetes on spot instances to provide on-demand compute
    3. https://pangeo.io/deployments.html#pangeo-provided-cloud-deployments
2. NVIDIA
    1. Large Graphics Processing Unit (GPU) maker
    2. Enabling data science on GPUs using dask
    3. http://matthewrocklin.com/blog/2019/01/13/dask-cudf-first-steps
3. Anaconda
    1. Platform and dependency manager for Python data science
    2. Supports dask as part of core value proposition
4. Quansight
    1. ​Open source software support and consulting focused on data science

### Governance

From https://github.com/dask/governance:

"Traditionally, Project leadership was provided by a BDFL (Matthew Rocklin) and a subset of Contributors, called Core Developers, whose active and consistent contributions have been recognized by their receiving ownership rights over the GitHub organization. In general all Project decisions are made through consensus among the Core Developers with input from the Community. The BDFL can, but rarely chooses to, override the Core Developers and make a final decision on a matter."

However, as the Dask Project matured, a more formal governance model was adopted. There remains a benevolent dictator-for-life (BDFL), and his or her final authority is realized as an infrequent override or tie-break or when the Steering Council requests a decision. The Steering Council is made up of the owners of the Github organization (see https://github.com/orgs/dask/people, https://github.com/dask/dask/issues/3223). The members of the Council work with the BDFL and are expected to be contributors with expert knowledge of the project. Their goal is to ensure "the long-term well-being of the project, both technically and as a community." Conflicts of interest involving any member of the Council must be disclosed, and recusal from voting is required. If the BDFL is recused, a temporary BDFL is appointed.

### Metrics

Dask uses TravisCI and Appveyor for continuous integration and reports unit test code coverage of around 94%. Metrics of success for the community include the number of active contributors, the integrations with dask that other open-source scientific python communities support, and the level of corporate use and sponsorship.
