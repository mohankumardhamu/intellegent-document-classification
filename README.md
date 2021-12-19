# intellegent-document-classification
Document Classification using Amazon S3, Amazon Textract and Amazon Comprehend

# List of AWS services used
1. Amazon S3 -> To store the training data which contains the category and its relevant document text in a csv format.
2. Amazon Textract -> To get the text containing in a PDF document.
3. Amazon Comprehend -> In this service we will provide the training data csv and provide input/output details pointing to Amazon S3. Then we will create a job based on the custom classification (the model built based on the csv file). This job will read the text files in the s3 bucket and provide a .jsonl file in which the category is mentioned with a score value.
