Apache Pig is a data manipulation tool that is built over Hadoop’s MapReduce. Pig provides 
us with a scripting language for easier and faster data manipulation. This scripting language 
is called Pig Latin. 
 
Before proceeding you need to make sure that you have all these pre-requisites as follows. 
1) Hadoop Ecosystem installed on your system and all the four components i.e. DataNode, 
NameNode, ResourceManager, TaskManager are working. If any one of them randomly 
shuts down then you need to fix that before proceeding. 
2) Download the Pig version 0.17.0 tar file from the official Apache pig site. 
3) Then extract the tar file. 
4) Rename the extracted file as pig and move it to the home directory. 
5) Then, update.bashrc add the below at the end of the file,
export PIG_HOME=/home/nmamit/pig export PATH=$PATH:/home/nmamit/pig/bin 
export PIG_CLASSPATH=$HADOOP_HOME/conf 
export HIVE_HOME=/home/nmamit/hive export PATH=$PATH:$HIVE_HOME/bin 
export SPARK_HOME=/home/nmamit/spark export 
PATH=$PATH:$SPARK_HOME/bin:$SPARK_HOME/sbin export 
PYSPARK_PYTHON=/usr/bin/python3 
1.Develop a word count program using Pig Latin. 
Wordcount with random lines saved as input.txt 
2.Develop a program to calculate the following for weather dataset using 
Pig Latin: 
a. Load the entire file of wether.txt and name it records. 
b. Filter the records by temperature! = 9999 AND quality IN (0, 1, 4, 5, 9). 
c. Grouping the records. 
d. Finding the maximum temperature. 
Weather dataset with year temperature and quality as columns 
Move to working directory, change the directory.
cd Desktop 
In that create a directory named rmmbdalab.
cd rmmbdalab 
To enter into interactive grunt shell, execute the command:
pig -x local
Now create a text file with some input data in the current working directory:
Example: wordcount.txt  
gedit wordcount.txt  
gedit weather.txt

