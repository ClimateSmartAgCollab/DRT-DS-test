# DRT-DS-test
The test data-store for the Data Request Tracker

# Notes

## owner_table.csv
A new dataowner will need to add themselves to the owner_table.
Enter in a unique username. This username should not be changed. Add the associated email address which is the contact email of the dataset owner. Email addresses can be changed. The dataset owner (or dataset steward) will receive all communications about the dataset and they will also be able to generate the unsigned licenses.

## linktable.csv
To create a link and connect it to a questionnaire to share with potential data requestors an owner will have to add an entry to the linktable. To start, the owner generates a new random link and enters it in the table. The data owner (or steward) then fills out the rest of the table accordingly:

* link - random link that can be shared with data requestors that starts them answering the right questionnaire.
* questionnaire_id - which questionnaire the data requestor will answer.
* owner_id - which owner the answers to the questionnaire will be given.
* expiry - rather than deleting a link, the link is expired here. Enter the date the link is no longer valid from.
* data_label - for summary statistics, the data owner can create a comma separated list of tags for their own use.

If the data owner wants to use the same questionnaire but share it for different datasets (and wants summary statistics available) the data owner can create multiple entries referencing the same questionnaire but with different data_label values.


