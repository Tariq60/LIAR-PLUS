## LIAR-PLUS
The extended LIAR dataset for fact-checking and fake news detection released in our paper:
[Where is Your Evidence: Improving Fact-Checking by Justification Modeling. Tariq Alhindi, Savvas Petridis and Smaranda Muresan](http://aclweb.org/anthology/W18-5513). In Proceedings of the First Workshop on Fact Extraction and VERification (FEVER) Brussels, Belgium November 1st, 2018.
<br><br>
This dataset has evidence sentences extracted automatically from the fact-checking articles written by the journalist in Politifact in order to provide a benchmark for evidence retrieval and show empirically that including evidence information in any automatic fake news detection methods results in superior performance to any method lacking such information.
<br><br>
Below is the description of the TSV file taken as is from the original [LIAR dataset](https://www.cs.ucsb.edu/~william/data/liar_dataset.zip). We added an new column at the end that include the extracted justification.
<br>
- Column 1: the ID of the statement ([ID].json).
- Column 2: the label.
- Column 3: the statement.
- Column 4: the subject(s).
- Column 5: the speaker.
- Column 6: the speaker's job title.
- Column 7: the state info.
- Column 8: the party affiliation.
- Columns 9-13: the total credit history count, including the current statement.
  - 9: barely true counts.
  - 10: false counts.
  - 11: half true counts.
  - 12: mostly true counts.
  - 13: pants on fire counts.
- Column 14: the context (venue / location of the speech or statement).
- **Column 15: the extracted justification**
<br>
Note that we do not provide the full-text verdict report in this current version of the dataset,
but you can use the following command to access the full verdict report and links to the source documents:
wget http://www.politifact.com//api/v/2/statement/[ID]/?format=json
<br><br>
The original sources retain the copyright of the data.
<br>
Note that there are absolutely no guarantees with this data,
and we provide this dataset "as is",
but you are welcome to report the issues of the preliminary version
of this data.
<br>
You are allowed to use this dataset for research purposes only.
<br>
Kindly cite our paper if you find this dataset useful.

@inproceedings{alhindi2018your,<br>
  title={Where is your Evidence: Improving Fact-checking by Justification Modeling},<br>
  author={Alhindi, Tariq and Petridis, Savvas and Muresan, Smaranda},<br>
  booktitle={Proceedings of the First Workshop on Fact Extraction and VERification (FEVER)},<br>
  pages={85--90},<br>
  year={2018}<br>
}
