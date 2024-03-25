# ML Ops with Vertex AI for enterprises

Enterprises frequently have specific requirements, especially around security and scale, that are 
often not addressed by other examples. In this example we demonstrate machine learning use case 
implementation that respects typical security requirements, and that includes that automation to 
allow larger organizations achieve scale in terms of number of models.

## Contents of this example

We provide three Vertex AI pipelines examples based on different technologies: 

- [KFP pipeline](src/kfp_pipelines/README.md) using Vertex AI custom training
- [KFP pipeline using BigQuery ML](src/bqml_pipeline/README.md)
- [TFX pipeline](src/tfx_pipelines/) using Vertex AI custom training. In this case, a set of notebooks is also provided for the experimentation phase:
    1. [experimentation.ipynb](01-experimentation.ipynb) covers the development process, where the features, the model and the training process are defined.
    2. [cicd.ipynb](02-cicd.ipynb) covers the the CI/CD process that tests the code produced in the experimentation phase, and trains a production-ready model.
    3. [prediction.ipynb](03-prediction.ipynb) cover the deployment process to make the model available, for example on a Vertex AI Endpoint or through Vertex AI Batch Prediction.

Once you have reviewed the pipelines, you can go on with these advanced steps to set up the automated environments and the CI/CD process using Github.

1. [Environments](doc/01-ENVIRONMENTS.md) covers how to automate the environments deployments using Terraform.
1. [GIT Setup](doc/02-GIT_SETUP.md) covers how to configure a Github repo to be used for the CI/CD process.
1. [MLOps end2end process](doc/03-MLOPS.md) cover test the automated MLOps end2end process.

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>


## License

All solutions within this repository are provided under the
[Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license. Please see
the [LICENSE](/LICENSE) file for more detailed terms and conditions.

## Disclaimer

This repository and its contents are not an official Google Product.
