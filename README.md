<b>Getting Set-Up</b>

Before we start, Visual Studio Code will often try to be helpful and pop up additional extensions to load. Some extensions interfere with others, so use caution 
when installing more extensions. Here is an example of a suggested extension that I ignored: 

  <img width="357" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/046afd4d-2ce2-43cd-a97e-50c17c0539d8">


1. Create a new repository from this template by clicking on the green <b>Use this template</b> button and selecting
   <b>Create a new respository</b>.

   <img width="501" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/884e64b4-f9bc-4680-8ead-ee2bc1ef121a">

   <img width="148" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/43dce32c-1ef1-4c83-a4d5-cc41ab092137">

 
2. On the <b>Create a new repository</b> page, select your GitHub username for the <b>Owner</b> and add in a name for your repository.

   <img width="546" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/f05e0df9-a393-441e-9c93-93407f65567c">

3. If you want to include the solution files as well, you will want to select <b>Include all branches</b>.

   <img width="421" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/3b14efda-3848-43d8-a04f-031261ad7123">


4. Then click the green <b>Create repository</b> button to create a new repository using the template repository.

5. Once the new respository is create, copy the URL to use in Visual Studio Code.

   <img width="341" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/d1be1a60-5248-41b9-95e8-140f5ee95cef">


6. In Visual Studio Code, click on the <b>Source Control</b> tab, then click <b>Clone Repository</b>.

   <img width="247" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/22a58636-7edc-4478-a759-c50dfeeaedf3">

7. Paste the respository URL into the Visual Studio search window. You'll be prompted to choose the location to store the files and whether or not you trust
   the authors of the folder. 

   <img width="478" alt="image" src="https://github.com/clfurman/PatternMatchingSealed/assets/65421044/93d623e8-1c87-4dac-82a2-590dc8748568">

8. Under Run Configurations add <code>--enable-preview --source 21</code> to VM Options.
   

<hr>


1. Open the <b>Meteorite_Landings.csv</b> file and identify the fields you will need to represent in your <code>Meteor</code> record and <code>GeoLocation</code> record. The starter files store dates as <code>String</code> objects.
   NOTE: each row represents an individual meteor and each column represents the data we know about the meteor.
   This data is <bold>immutable data </bold>. Therefore a record is the correct type of storage. 
   <img width="700" alt="image" src="https://github.com/clfurman/MeteoriteDataProject/assets/65421044/0658b41c-bbd6-435a-81b7-172043d7f83c">


2. Create your <code>Meteor</code> record. To add a new Java file to the project, click on the the file icon with the plus symbol.

   <img width="250" alt="image" src="https://github.com/clfurman/MeteoriteDataProject/assets/65421044/5ee76669-712f-49b9-ab35-b814ff6340c3">

3. Be sure to add your package at the top of the files and save the file as <b>Meteor.java</b>.
   Since the <code>GeoLocation</code> contains the latitude and longitude values, we don't actually need to store the latitude and longitude values separately.
   You only need to store 8 fields. 
4. Create the <code>GeoLocation</code> record. Be sure to add your package at the top of the file. It will contain two fields. Save the file as <b>GeoLocation.java</b>
5. Modify the runner class, <b>SIGCSEMeteor2.java</b> to ensure the file path for the <b>Meteorite_Landings.csv</b> is where you saved it on your computer.
    Run the <b>SIGCSEMeteor2.java</b> main method to import the data and add the meteors with a mass less than 5000 to a new list. ​
6. Your solution may be similar to those in the <b>Solution_Files</b> branch.
