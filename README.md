<!-- Header block for project -->
<hr>

<div align="center">

![logo](https://user-images.githubusercontent.com/3129134/163255685-857aa780-880f-4c09-b08c-4b53bf4af54d.png)

<h1 align="center">Unity SDS Processing Service (U-SPS)</h1>
<!-- ☝️ Replace with your repo name ☝️ -->

</div>

<pre align="center">The SPS is the component of the Unity system responsible for executing data processing of scientific workflows at scale.</pre>
<!-- ☝️ Replace with a single sentence describing the purpose of your repo / proj ☝️ -->

<!-- Header block for project -->

[INSERT YOUR BADGES HERE (SEE: https://shields.io)] [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) [![SLIM](https://img.shields.io/badge/Best%20Practices%20from-SLIM-blue)](https://nasa-ammos.github.io/slim/)
<!-- ☝️ Add badges via: https://shields.io e.g. ![](https://img.shields.io/github/your_chosen_action/your_org/your_repo) ☝️ -->

[INSERT SCREENSHOT OF YOUR SOFTWARE, IF APPLICABLE]
<!-- ☝️ Screenshot of your software (if applicable) via ![](https://uri-to-your-screenshot) ☝️ -->

This repository contains high level information (such as documentation, change log, etc.) about the U-SPS software stack. The actual U-SPS code is contained within the following set of GitHub repositories:
* [U-SPS Prototype](https://github.com/unity-sds/unity-sps-prototype): Terraform scripts to deploy the U-SPS cluster (either the HySDS or Airflow implementations)
* [U-SPS Workflows](https://github.com/unity-sds/unity-sps-workflows): Examples of CWL workflows that can be executed on a U-SPS cluster
* [U-SPS API](https://github.com/unity-sds/unity-sps-api): The API used to manage a U-SPS cluster
* [U-SPS Register Job](https://github.com/unity-sds/unity-sps-register_job): Implementation of the WPS-T API with respect to the supported U-SPS backe-ends

## Features

*  The U-SPS enables deployment and execution of arbitrary scientific data processing algorithms through the standard OGC WPS-T API ("Open Geospatial Consortium Web Processing Service - Transactional Abstract Programming Interface")
   * Deploying and undeploying a science algorithm via the "/processes" endpoint
   * Executing and monitoring a job execution via the "/jobs" endpoint
   * Retrieving a job output via the "/results" endpoint
* Scientific data processing workflows are encoded via the CWL ("Common Worflow Language") standard
* The U-SPS includes an API to manage the computing resources of the cluster (such as scaling up and down the number of computing nodes)
* Internally, the U-SPS is composed of a system of interacting applications packaged as Docker containers and deployed into a Kubernetes cluster via a set of Terraform scripts.
*  The U-SPS supports multiple possible implementations. The two currently available are based on HySDS (Hybrid Science Data System) and Apache Airflow
<!-- ☝️ Replace with a bullet-point list of your features ☝️ -->

## Contents

* [Quick Start](#quick-start)
* [Changelog](#changelog)
* [FAQ](#frequently-asked-questions-faq)
* [Contributing Guide](#contributing)
* [License](#license)
* [Support](#support)

## Quick Start

This guide provides a quick way to get started with our project. Please see our [docs](https://unity-sds.gitbook.io/docs/developer-docs/science-processing) for a more comprehensive overview.

### Requirements

* [INSERT LIST OF REQUIREMENTS HERE]
  
<!-- ☝️ Replace with a numbered list of your requirements, including hardware if applicable ☝️ -->

### Setup Instructions

1. [U-SPS Setup](https://unity-sds.gitbook.io/docs/developer-docs/science-processing/docs/admin-guide/cluster-provisioning-with-terraform) 
   
<!-- ☝️ Replace with a numbered list of how to set up your software prior to running ☝️ -->

### Run Instructions

1. [INSERT STEP-BY-STEP RUN INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your run instructions, including expected results ☝️ -->

### Usage Examples

* [Tutorial: Executing the L1B workflow](https://unity-sds.gitbook.io/docs/developer-docs/science-processing/docs/developers-guide/tutorial-execution-of-the-l1b-cwl-workflow-via-the-wps-t-api)
* [Tutorial: Using Job Labels](https://unity-sds.gitbook.io/docs/developer-docs/science-processing/docs/developers-guide/job-labels)
* [Tutorial: Testing the SPS Prewarm API](https://unity-sds.gitbook.io/docs/developer-docs/science-processing/docs/developers-guide/manual-verification-testing-the-sps-prewarm-api)

<!-- ☝️ Replace with a list of your usage examples, including screenshots if possible, and link to external documentation for details ☝️ -->

### Build Instructions (if applicable)

1. [INSERT STEP-BY-STEP BUILD INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your build instructions, including expected results / outputs with optional screenshots ☝️ -->

### Test Instructions (if applicable)

1. [INSERT STEP-BY-STEP TEST INSTRUCTIONS HERE, WITH OPTIONAL SCREENSHOTS]

<!-- ☝️ Replace with a numbered list of your test instructions, including expected results / outputs with optional screenshots ☝️ -->

## Changelog

See our [CHANGELOG.md](CHANGELOG.md) for a history of our changes.

See our [releases page]([INSERT LINK TO YOUR RELEASES PAGE]) for our key versioned releases.

<!-- ☝️ Replace with links to your changelog and releases page ☝️ -->

## Frequently Asked Questions (FAQ)

[INSERT LINK TO FAQ PAGE OR PROVIDE FAQ INLINE HERE]
<!-- example link to FAQ PAGE>
Questions about our project? Please see our: [FAQ]([INSERT LINK TO FAQ / DISCUSSION BOARD])
-->

<!-- example FAQ inline format>
1. Question 1
   - Answer to question 1
2. Question 2
   - Answer to question 2
-->

<!-- example FAQ inline with no questions yet>
No questions yet. Propose a question to be added here by reaching out to our contributors! See support section below.
-->

<!-- ☝️ Replace with a list of frequently asked questions from your project, or post a link to your FAQ on a discussion board ☝️ -->

## Contributing

Interested in contributing to our project? Please see our: [CONTRIBUTING.md](CONTRIBUTING.md)

## License

See our: [LICENSE](LICENSE)

## Support

[INSERT CONTACT INFORMATION OR PROFILE LINKS TO MAINTAINERS AMONG COMMITTER LIST]

<!-- example list of contacts>
Key points of contact are: [@github-user-1](link to github profile) [@github-user-2](link to github profile)
-->

<!-- ☝️ Replace with the key individuals who should be contacted for questions ☝️ -->
