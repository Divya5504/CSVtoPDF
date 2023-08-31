# CSVtoPDF
How to Convert CSV to PDF in Boomi

AtomSphere currently does not support PDF conversion natively, but in this article we use custom scripting wherein we make use of third party libraries for PDF conversion.

Please note that you could achieve this conversion with your own choice of custom libraries. 

In this article we used the following java libraries:

Apache PDFBox
Boxable
Apache Commons CSV

...................................................................................
- Boxable 1.5 (boxable-1.5.jar) 
https://github.com/dhorions/boxable
- Commons CSV 1.2 (commons-csv-1.2.jar)
https://commons.apache.org/proper/commons-csv/
- Fontbox 2.0.0 (fontbox-2.0.0.jar)
https://pdfbox.apache.org/
- Guava 18.0 (guava-18.0.jar)
https://github.com/google/guava
- PDFBox 2.0.0 (pdfbox-2.0.0.jar)
https://pdfbox.apache.org/
- PDFBox Tools 2.0.0 (pdfbox-tools-2.0.0.jar)
https://pdfbox.apache.org/
.........................................................
  Requirements for the input CSV:

Ensure that your input CSV has the following settings:

It must be a comma delimited Flat file with double quotes as text qualifier.
Make you sure you combine CSV rows into a single document before sending through the script
 

Setup Instructions:

Upload all JAR files: 
Go to Manage Account Libraries page in Atomsphere platform (Settings > Account Information and Setup > Account Libraries) to upload all the JAR files mentioned above.

Create a Custom Library Component of type Scripting with these JAR files.


Use the following custom script wherever you need CSV to PDF conversion in your process.
Make sure to deploy the custom library along with your process(es).


Here is a sample process that converts an input CSV into PDF:

Get it Now

 

NOTE: The script in this example process is customizable to your requirements.

 

 


