# CancerDataServices-CDS_to_SRA
This script will take a CDS submission template and create a dbGaP SRA submission template.

To run the script on a complete and validated [CDS v1.3.1 validated submission template](https://github.com/CBIIT/CancerDataServices-SubmissionValidationR), run the following command in a terminal where R is installed for help.

```
Rscript --vanilla CDS_to_SRA.R --help
```

```
Usage: CDS_to_SRA.R [options]

CDS-CDS_to_SRA v2.0.0

Options:
	-f CHARACTER, --file=CHARACTER
		A validated dataset file (.xlsx, .tsv, .csv) based on the template CDS_submission_metadata_template-v1.3.1.xlsx

	-t CHARACTER, --template=CHARACTER
		A dbGaP SRA metadata template, 'phsXXXXXX'

	-h, --help
		Show this help message and exit
```

An example usage would be the following:

```
Rscript --vanilla CDS_to_SRA.R -t phsXXXXXX.xlsx -f test_files/a_all_pass_validated_CDS-v1.3.1.xlsx 
The SRA submission file is being made at this time.


The dbGaP SRA metadata submission has been created here: test_files/a_all_pass_validated_CDS-v1.3.1_SRA_submission_2022_09_12.xlsx.
```

If there are any errors or problems with the file, it will write out the possible issues. Most of these should not occur as these submission manifests should be valid based on the [CDS-SubmissionValidatoR](https://github.com/CBIIT/CancerDataServices-SubmissionValidationR).
