# ExtendCD BulkJob Creation #

Java utility to create bulk CI jobs in CI server 

## Usage of the ExtendCD BulkJob Creation Utility ##

This utility is aimed at automating the process of creating a large number of CI jobs in CI server.One can run this utility to 
create n number of branch CI jobs in CI server .It helps reduce the effort involved in creating CI build jobs manually for each 
time when you cut the release.

## Benefits ##

If this jenkins utility would have not been there then User has to manaully create CI branch jobs for each sprint which requires lot
of effort.

## Tools and Softwares Required ##

```
    * Jenkins Core 1.580 or above
	* Maven 3.X
    * Java JDK7 or JDK8
	* Eclipse IDE
	
```

## Package ##

```    
       Method1
	   =======
	   Import Gitlab project to Eclipse
       In the Project Explorer section, right click and choose "Import Project"
	   Under General, pick Existing Projects into Workspace
	   Click Next and browse the root directory of your project and click Finish
	   After you have a project in Eclipse that is connected to Gitlab, you can run it as maven project which will create jar file in the target folder
     
	  Method2
	  =======
	  Checkout the sourcecode into your local machine and navigate to the path where your sourcecode is present and from the root directory,
	  where pom.xml resides invloke mvn clean install 
	 
	  Note: the first time this command is invoked, many downloads will occur and it will take quite some time.
```

## Using the utility ##

```
     *For creating the Jenkins Job simply create a freestyle job in jenkins server, 
	 *Add the Execute windows batch command in the job and execute the jar with the jar location and command line arguments.
```
