# Extract-data-using-UIPATH
Automate data extraction from structured & unstructured documents. Get up to 98% accuracy.

Now we can discuss step by step Bot development.
 
Step 1
 
Open UiPath Studio -> Start -> New Project-> Click Process
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Step 2
 
Now, create new Blank Process, and name it  UiPdfSpecific and give your description.

 
Step 3
 
After that UiPath studio creates the project UiPdfSpecific with supporting files.
 

 
Step 4
 
Next, for extracting the specific text in PDF document, create a new sequence workflow named ReadSpecificData:
 

 

 
Create 5 variables, InvoiceNo as a String Data Type, OrderNo as a Int32 Data Type, InvoiceDate as a String Data Type, DueDate as a String Data Type, TotalDue as a String Data Type.

 
For getting the invoice number, Click Activities -> search GetText activity->Drag and drop into sequence,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Click the Indicate in screen, select the Invoice number:
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Set the element value property as InvoiceNo:
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Similarly, for getting the ordernumber, click Activities -> search GetText activity->Drag and drop in to sequence, click the Indicate in screen, select the Order Number, Set the element value property as OrderNo,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Similarly, for getting the invoice date, click Activities -> search GetText activity->Drag and drop in to sequence, click the Indicate in screen, select the Invoice date, set the element value property as InvoiceDate,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Similarly, for getting the due date, click Activities -> search GetText activity->Drag and drop in to sequence, click the Indicate in screen, select the Due Date, set the element value property as DueDate,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Similarly, for getting the Total Due, click Activities -> search GetText activity->Drag and drop in to sequence, click the Indicate in screen, select the Total Due, set the element value property as Total Due,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Click Activities -> search Message Box activity->Drag and drop into sequence and set the text as:
 
"InvoiceNo : " + InvoiceNo.ToString+Environment.NewLine +"Order No: "+OrderNo.ToString+Environment.NewLine +"Invoice Date :"+InvoiceDate.ToString+ Environment.NewLine +"Due Date :"+DueDate.ToString+ Environment.NewLine+"Total Due :"+ TotalDue.ToString 
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
Step 5
 
For running your project, Select debug file -> Run. The output of the UiPdfSpecific project is,
 
Extract Specific Data From PDF Automation Using UiPath Studio
 
