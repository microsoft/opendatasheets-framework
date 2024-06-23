# Open Datasheets

The Open Datasheets framework is a simple, standardized no-code way to document datasets. It is inspired by the concept of [datasheets for datasets](https://arxiv.org/abs/1803.09010) and [Understanding Machine Learning Practitioners' Data Documentation Perceptions, Needs, Challenges, and Desiderata](https://dl.acm.org/doi/10.1145/3555760) research papers. The framework is designed to be both machine-readable and human-readable, serving as a tool for dataset creators to document their datasets and for dataset consumers to understand the datasets they are using.

By integrating directly with GitHub, the framework allows you to create, edit, and export your Open Datasheets directly to GitHub. It leverages the widely used [Data Package](https://specs.frictionlessdata.io/data-package/) standard to describe the dataset and its metadata, benefiting from the support of various tools and libraries. Additionally, it extends this standard to incorporate responsible AI aspects into the dataset documentation, derived from [Microsoft’s Aether data documentation](https://www.microsoft.com/en-us/research/uploads/prod/2022/07/aether-datadoc-082522.pdf). This includes information about the dataset's provenance, collection process, privacy and security considerations, and more.

Adhering to good data documentation practices is crucial for responsible AI, as it helps assess how a dataset may impact machine learning models and other solutions derived from it.

The primary goal of this framework is to facilitate dataset documentation, promote transparency, and aid dataset creators and consumers in making informed decisions about the suitability of specific datasets and the limitations they may have. This framework achieves its goal by applying a no-code approach, making it accessible to both non-technical data producers and those with a technical background. For more detailed information, you can refer to our paper titled "[Open Datasheets: Machine-readable Documentation for Open Datasets and Responsible AI Assessments](https://arxiv.org/abs/2312.06153)".

# Try the No-Code App
We have created a no-code web tool to help you create, edit, generate, and export an Open Datasheets `datapackage.json` file for your datasets directly to/from GitHub. You can also work with files located locally on your computer. 

You can try it out here: [https://microsoft.github.io/opendatasheets](https://microsoft.github.io/opendatasheets).

With the no-code tool, you have the ability to:
- Create a new Open Datasheets datapackage from scratch.
- Generate a new Open Datasheets datapackage from data located on GitHub or a local file.
- Modify an existing Open Datasheets datapackage file from GitHub or a local file.
- Save an Open Datasheets datapackage file to GitHub or locally.


DEMO:

![demo](./assets/demo.gif)

# Top level schema

| Property | Description | Key Elements for Fostering Responsible AI |
| --- | --- | --- |
| name | The name of the data package. |  |
| title | The title of the data package. | |
| description | The description of the data package. |  |
| version | The version of the data package. |  |
| created | The date when the data package was created. |  |
| licenses | The licenses under which the data package is distributed. |  |
| sources | The sources from which the data package is derived. |  |
| resources | The resources included in the data package. |  |
| contributors | The contributors to the data package. | |
| privacy | The privacy considerations for the data package. | &#x2705; |
| security | The security considerations for the data package. | &#x2705; |
| procedures | The collection, processing, and update procedures for the data package. | &#x2705; |
| use | The permitted use of the data package. | &#x2705; |

For the complete schema, please refer to the [Open Datasheets schema](./examples/datapackage.json).

For more detailed information about the responsible AI properties, such as collection procedures, privacy, and security considerations, please refer to the [Open Datasheets paper](https://arxiv.org/pdf/2312.06153).

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.

# Citation

If you use the Open Datasheets framework in your research or project, please cite our paper:

```
@article{roman2023open,
  title={Open Datasheets: Machine-readable Documentation for Open Datasets and Responsible AI Assessments},
  author={Roman, Anthony Cintron and Vaughan, Jennifer Wortman and See, Valerie and Ballard, Steph and Schifano, Nicolas and Torres, Jehu and Robinson, Caleb and Ferres, Juan M Lavista},
  journal={arXiv preprint arXiv:2312.06153},
  year={2023}
}
```

