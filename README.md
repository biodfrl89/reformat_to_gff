# reformat_to_gff
This script is designed to take BLAST m6 output file, hmmer output file, STAR joints output table or manual curation and reformat them to GFF format. The script is designed in Python 3.10 and uses modules from Pandas, Biopython and argparse, all of which must be installed for the script to run.

## Syntax

blastm6_to_gff.py --file [FILE] --source [SOURCE] --bitscore [BITSCORE] --input_type [INPUT_TYPE]

## Options

| Options | Description | 
| --- | --- |
| file | The input file produced by blast with output format 6 (tabular). Mandatory. |
| source | The mode in which blast was performed, e.g. blastn, blastp, tblastx, or another. Mandatory. |
| bitscore | Bitscore obtained by blast. Used to add a level of filter to the result. If 0 (default), all results will be maintained. Optional. |
| input_type | The type of the input file. It must be one of the following: m6, hmmer, star_joints, manual. Mandatory. |

