# JPDB
Insert data from Web using JPDB

Create this project using NetBeans IDs Steps are:
1) Open the NetBeans
2) Click on New Projects
3) Select Htmlapplication and click on next button
4) Enter Project Name and selet project location and click on next button
5) Then select No-Site Template then click on next and then click on Finish button.
So that Html Application Project is Created with default index.html file

Create Web Form for inserting the data into JsonPowerDB
There 2 Methods.
First Method is Use Javascript Ajax function to exceute Put Command to insert the Data into JPDB using Api's
Second Method is Use to Pre-defined Script library "<script src="http://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js"></script>" that have pre-defined method to exceute Api Commands.

Use the Files to Run the Files

For Run the Html Application file. You need to Add Netbeans Connector Extension. if you don't add extension then application first ask to add extension.
Steps are for adding Netbeans Connector Extension
1) Go to the browser and click on the 3 dots then click on setting
2) click on the Extension
3) click on the left site and click on Open Chrome Web store
4) Search for "NetBeans Connector" and click on the add button 

Explain the Script Code here for First Method
When User Click on the submit button then saveEmployee() is called. Method have some sub Methods like

function saveEmployee(){
//Validation

//Create PUTJsonStr reuqest

//ExceuteCommand to insert the data

//Reset the form for another save the responce
}

1) Validation Method have Input Field value. if Input field is blank then return otherwise create json object and return the JsonStr object with value
2) PutJsonStr Request have 4 parameteres a) Connector Token b) JsonStr Object c) Database Name d) Relation Name. This Methods return the JsonString object that have "PUT" Command
3) Run the  executeCommand() method that have 3 parameters that is a) PutJsoStr object b)Base Api Url  c)End Api Url. This Method is used to insert the data for particular database and return the successfully message.
4) Reset Form method is use to Reset the Input Field and make this field for another response.



Second Method is that to remove the CreatePutJsonStr method and ExceuteCommand() because Script library have pre-defined these methods so no need to create these method manually.
