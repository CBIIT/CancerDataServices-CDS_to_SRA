# CancerDataServices-CDS_to_SRA
This script will take a CDS submission template and create a dbGaP SRA submission template.

To run the script on a complete and validated [CDS v1.3.1 validated submission template](https://github.com/CBIIT/CancerDataServices-SubmissionValidationR), run the following command in a terminal where R is installed for help.

```
Rscript --vanilla CDS-File_CopieR.R --help
```

```
Usage: CDS_to_SRA.R [options]

CDS-CDS_to_SRA v.1.3.1

Options:
	-f CHARACTER, --file=CHARACTER
		A validated dataset file (.xlsx, .tsv, .csv) based on the template CDS_submission_metadata_template-v1.3.1.xlsx

	-t CHARACTER, --template=CHARACTER
		A dbGaP SRA metadata template, 'phsXXXXXX'

	-h, --help
		Show this help message and exit
```

An example usage would be the following:
