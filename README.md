# Assignment 03
## 1. Checking Pre-requisites Command: docker images Result:
![image](https://github.com/user-attachments/assets/e5dbe08a-4a50-450f-ba2b-70c7d49afe7f)


## 2. Verifing Containers
![image](https://github.com/user-attachments/assets/9e1a22b5-c40e-448f-b4a3-67e75b26d0a8)


## 3. Deploy the Cluster
![image](https://github.com/user-attachments/assets/a7ebeb29-ddef-43a6-97c5-e29ea549d0a7)


## 4. Verify Cluster Status
![image](https://github.com/user-attachments/assets/26a85cbc-83d8-40f3-b4ee-e6559f2b1c0c)


## 5. Create sample data file (sample.txt)
![image](https://github.com/user-attachments/assets/6be6ffbe-6d08-4952-bc91-050180c22f4b)


## 6. docker cp ./sample.txt namenode:/sample.txt
![image](https://github.com/user-attachments/assets/c6b24145-2afb-40b0-b9bf-f7ece4f6ce93)


## 7. docker exec -it namenode hdfs dfs -put /sample.txt /input 
![image](https://github.com/user-attachments/assets/68384ec5-1eb1-41cc-a1c8-a2de2ede438a)


## 8. docker exec -it namenode hadoop jar /opt/hadoop-3.2.1/share/hadoop/mapreduce/hadoop-mapreduce-examples-3.2.1.jar wordcount /input /output
![image](https://github.com/user-attachments/assets/1e719cf0-7fed-4103-8f03-db8df084fb2b)


## 9. docker exec -it namenode hdfs dfs -ls /output
![image](https://github.com/user-attachments/assets/30f45663-0eb7-4ec8-8e3a-9c087187704d)


## 10. docker exec -it namenode hdfs dfs -cat /output/part-r-00000
![image](https://github.com/user-attachments/assets/25ae2ff8-8641-43aa-882e-e33d232fe31a)








