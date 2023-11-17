# CS589_Fine-Tuning-based-on-2000-drug-examples



1) The data file is an XLSX file. We are going to convert it to JSONL format (JSON Lines.)

2) The JSONL file will be used for fine-tuning the model. We are also going to use this format:

3) To begin, use Pandas to transform the data into the desired format.

4) The code above sets the number of rows to read from the Excel file to 2000. This means that we are going to use a dataset of 2000 drug names to fine-tune the model.

5) It then gets the unique values in the 'Reason' column of the data frame, stores them in an array called reasons, assigns a numerical index to each unique value in the reasons array, and stores it in a dictionary called reasons_dict.


6) The script adds a new line and "Malady:" to the end of each drug name in the 'Drug_Name' column of the data frame. It concatenates a space and the corresponding numerical index from the reasons_dict to the end of each 'Reason' value in the data frame.

7) This is done to get the desired format:

1 Drug: <DRUG NAME>\nMalady:

8) For this example, we don't need the 'Description' column, that's why the script drops it from the data frame.

9) If the client disconnects before the job is completed, you may be asked to reconnect and check using the following command.

10) It confirms that a new fine-tuning job was created with the specified ID.
