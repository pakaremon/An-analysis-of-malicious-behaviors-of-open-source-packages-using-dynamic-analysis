| **Dataset**        | **Software Repository** | **Number of Packages** |
|--------------------|-------------------------|------------------------|
| Malicious Dataset  | npm                     | 1170                   |
| Benign Dataset     | npm                     | 1000                   |
| Total Dataset      | npm                     | 2170                   |

*Table 1: Number of software packages used in the machine learning application.*

This dataset is a raw analysis of the package-analysis tool.

Benign dataset: we get the top 1000 downloaded NPM packages

Malicious dataset: we get our sources from Vulert, Vulners, and OSV. 

After getting information about benign and malicious results, we query raw analysis results on Google BigQuery's package analysis. Then we explore this dataset and select three features for applying machine learning: commands, domains, and IP addresses. Note that these features are in the import and install phases. The type files are CSV.
