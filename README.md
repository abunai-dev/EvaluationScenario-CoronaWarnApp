# Case Study: Corona Warn App

This repository contains [Palladio](https://www.palladio-simulator.com/) software architecture models based on the German [Corona Warn App](https://www.coronawarn.app/en/). This app represents a large enterprise system of systems that has been commissioned by the German government, developed by SAP and Deutsche Telekom during the COVID-19 pandemic, and downloaded more than 48 million times. The contact tracing app exchanges keys between users via Bluetooth and handles highly sensitive data like COVID-19 test results.

We modeled all important functionality of the Corona Warn App, e.g., the exchange, download, and upload of keys, checking COVID-19 test results, requesting vaccination certificates, or gathering analysis data. The models in this repository are primarily used to evaluate confidentiality analysis and [Uncertainty Impact Analysis](https://github.com/abunai-dev/UncertaintyImpactAnalysis). However, other use cases for software architecture research evaluation are imaginable.

Please refer to the original publication: S. Hahner, R. Heinrich, and R. Reussner, "Architecture based Uncertainty Impact Analysis to Ensure Confidentiality", in *18th Symposium on Software Engineering for Adaptive and Self-Managing Systems (SEAMS)*, IEEE/ACM, 2023, doi: [10.1109/SEAMS59076.2023.00026](https://doi.org/10.1109/SEAMS59076.2023.00026)

The primary sources of the modeled information are:

- The [official documentation](https://github.com/corona-warn-app/cwa-documentation/blob/main/solution_architecture.md) of the open-source Corona Warn App
- Available [documentation](https://health.ec.europa.eu/system/files/2021-04/digital-green-certificates_dt-specifications_en_0.pdf) about digital COVID-19 certificates, also known as digital green certificates
- Documentation about the interfaces of the [CovPass Issuer](https://github.com/Digitaler-Impfnachweis/documentation)

## Branches

There are multiple branches that reflect different versions of the case study:

- The `main` branch contains the main case study with all Palladio models and additionally modeled confidentiality information
- The `uncertainty-impact-scenarios` branch contains 4 scenarios that have been used to evaluate the [Uncertainty Impact Analysis](https://github.com/abunai-dev/UncertaintyImpactAnalysis)

## Diagrams

Please use [Palladio](https://www.palladio-simulator.com/) to open the model files. To use the models in confidentiality analysis or uncertainty impact analysis, see the [installation guide](https://github.com/abunai-dev/UncertaintyImpactAnalysis).

In the following, we show the repository diagram and the allocation diagram. Click the images for a full size view.

### Repository diagram

[![Repository diagram](docs/repository.png)](https://raw.githubusercontent.com/abunai-dev/CaseStudy-CoronaWarnApp/main/docs/repository.png)

### Allocation diagram

[![Allocation diagram](docs/allocation.png)](https://raw.githubusercontent.com/abunai-dev/CaseStudy-CoronaWarnApp/main/docs/allocation.png)

## More information

For more information, please refer to [https://abunai.dev](https://abunai.dev).
