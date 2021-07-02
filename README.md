# JPDB
Insert data from Web using JPDB

**CRED Operation using JPDB**
**Project Description**

This Project have Create, Update, Read and delete operation using JPDB. In This method Data can be inserted, delete by row, Update Name & Email Address and get All data.
Also have 2 Methods to insert the data into JPDB. First is Create Manually Method to exceute the Api and Second is Use Pre-defined Javascript Library.

**About JsonPowerDB:**
JsonPowerDB is a Real-time, High Performance, Lightweight and Simple to Use, Rest API based Multi-mode DBMS. JsonPowerDB has ready to use API for Json document DB, RDBMS, Key-value DB, GeoSpatial DB and Time Series DB functionality.

**Benefits of using JsonPowerDB**
1) Simplest way to retrieve data in a JSON format.
2) Schema-free, Simple to use and In-Memory database.
3) It is built on top of one of the fastest and real-time data indexing engine - PowerIndeX.
4) It helps developers in faster coding, in-turn reduces development cost.

**Table Of Content**
Create Project using NetBeans
Define Both Method that are using for insert the data
How to Run the Project and how to ad NetBeans Connector Extension
Explain the Code


**Create this project using NetBeans IDs Steps are:**
1) Open the NetBeans
2) Click on New Projects
3) Select Htmlapplication and click on next button
4) Enter Project Name and selet project location and click on next button
5) Then select No-Site Template then click on next and then click on Finish button.
So that Html Application Project is Created with default index.html file

**Create Web Form for inserting the data into JsonPowerDB**
There 2 Methods.
First Method is Use Javascript Ajax function to exceute Put Command to insert the Data into JPDB using Api's
Second Method is Use to Pre-defined Script library "<script src="http://login2explore.com/jpdb/resources/js/0.0.3/jpdb-commons.js"></script>" that have pre-defined method to exceute Api Commands.

**Use the Files to Run the Files**

For Run the Html Application file. You need to Add Netbeans Connector Extension. if you don't add extension then application first ask to add extension.
Steps are for adding Netbeans Connector Extension
1) Go to the browser and click on the 3 dots then click on setting
2) click on the Extension
3) click on the left site and click on Open Chrome Web store
4) Search for "NetBeans Connector" and click on the add button 

**Explain the Script Code here for First Method**
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

Other Html page have Update, Delete and Get The data.

**JPDB Dashboard**
![image](https://user-images.githubusercontent.com/42262639/124275971-dada1200-db60-11eb-9bbd-98db8f42cde6.png)

**Insert Data**
![image](https://user-images.githubusercontent.com/42262639/124276011-e75e6a80-db60-11eb-8554-13b5babc458b.png)

**Show Data**
![image](https://user-images.githubusercontent.com/42262639/124275886-bf6f0700-db60-11eb-87f5-6f4c1a9c0fbb.png)

