Download Link: https://assignmentchef.com/product/solved-relational-databases-prog2111-assignment-1
<br>
<strong> </strong><strong>Objectives:</strong>

‐              To review file I/O basics

‐              To simulate a database service by using any method like the one given in the requirements OR by using Threads OR by simple File handling using multiple programs at the same time. <strong>Description:  </strong>

<strong>Method 1: </strong>

You will write a client‐server software system that demonstrates how a database system normally operates in a network environment. Generally, a database system runs as a service that responds to requests from an arbitrary list of sources. It is up to the database system to make sure data is secure and integrity is maintained. For example, only those sources that are permitted should access or update the data; and only one source can update data at a time – even though several sources may be requesting to update at the same time.

<strong>Method 2: </strong>

You can write a program that uses Threads for accessing and updating the same text file by many processes.




<strong>Method 3: </strong>

Write down programs that try to access the same file simultaneously running with each other. So, in effect you will be needing one program/application that creates a text file and then other applications/programs that can access and update the contents. You can use three applications/programs for this purpose.

<strong> </strong>

<strong>Requirements: </strong>

<ol>

 <li>The database file consists of records with the following fields:

  <ol>

   <li>MemberID (as an integer)</li>

   <li>FirstName (as a variable length string) C. LastName (as a variable length string)</li>

   <li>DateOfBirth (as a Date format supported by your OS)</li>

  </ol></li>

</ol>




<ol start="2">

 <li>Write a server program that will run continuously, listening for requests to write to the database. There are only 3 requests that the server can respond to:

  <ol>

   <li>INSERT ‐ allows the insertion of new data. The data should be provided only as the FirstName, LastName and DateOfBirth. The MemberID is automatically generated and written to the file with the rest of the data. The automatically generated MemberID must be sequential.</li>

  </ol></li>

</ol>

The server should only handle up to 40,000 records. This means that IDs of 1‐40,000 would be valid.

If the INSERT command is not successful, an error should be returned to the client.

<ol>

 <li>UPDATE – allows the modification of existing records. The client must provide a valid MemberID, FirstName, LastName and DateOfBirth. Even though the data may not change, all four values should be in the parameter list.</li>

</ol>

If the UPDATE command is not successful, an error should be returned to the client.

<ol>

 <li>FIND – allows a client program to get the information of a specific MemberID. The server should return all four data fields.</li>

</ol>

If the FIND command is not successful, an error should be returned to the client.




<ol start="3">

 <li>Write a client program that can be run multiple times concurrently from one or more computers. The purpose of this program is to randomly create the data that will be written to the database and to demonstrate that you can handle multiple requests simultaneously.</li>

</ol>




<ol start="4">

 <li>Write a client program that can query the database (use the FIND command) and will allow you to update a specific record.</li>

</ol>




<strong>Hand in: </strong>

<strong>Method 1 Submission: </strong>

<ol>

 <li>The Server command definitions/protocol document</li>

 <li>All source code</li>

 <li>Installation and usage instructions</li>

 <li>Document stating any problems or deficiencies (bug list) in the submitted program.</li>

</ol>




<strong>Method 2 Submission: </strong>

<ol>

 <li>All source codes</li>

 <li>Usage instructions</li>

</ol>




<strong>Method 3 Submission: </strong>

<ol>

 <li>All source codes</li>

 <li>Usage instructions</li>

</ol>




Please discuss if you are still unclear about the requirements by dropping an email. I will be available for discussion on our class day that is Tuesday September 22,2020 after our regular class for some time.