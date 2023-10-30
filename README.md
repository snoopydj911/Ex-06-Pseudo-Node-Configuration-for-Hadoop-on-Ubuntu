# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/e1cbafff-3772-4eb1-aa74-1cf7de1033d8)


2.	Install java1.8 in folder /usr/local
   ![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/3afdd0ff-c77f-40c5-93a2-733a8c354afa)

3.	Install Hadoop
   ![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/e4b32179-a598-4ff8-8ca1-0a6a3bdf1040)


7.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/e6817394-1d64-4834-861b-70db6c0bf2ad)

 
8.	Set hadoop environment variables: Include the following lines /etc/profile file
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/5aedd4db-8b1d-4743-aa73-751014006f54)


9.	Run the.bashrc & profile files from the $ prompt for updating the changes
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/3b71c2ea-8d17-4ec8-8f73-8b242dd581c0)
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/2b4d4fef-a41f-4c93-bd76-ac796a4c7939)





$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/a553ecb7-58fc-4e5d-9ff9-0d4f9f27da77)



b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)
![image](https://github.com/snoopydj911/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/122033587/c37367a3-624d-4c74-81e3-c0bf43e309a9)


 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags



c)	mapred-site.xml

 

Include the following lines in mapred-site.xml file
 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file


e)	yarn-site.xml
Include the following lines in yarn-site.xml file
8.	Format the Hadoop File system implemented on top of the local file system using

9.	Start Hadoop using


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:


11.	Create a directory ‘/input’ in HDFS


12.	Copy the input files into the distributed file system

13.	Run some of the examples provided


14.	Examine the output files
Copy the output files from the distributed file system to the local file system and examine them:
 
or
View the output files on the distributed file system

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
