# ElasticSearch/GlusterFS
Elasticsearch / GlsuterFS / Cassandra:
>> Create a 3 node elasticsearch cluster with the name `pp_elasticsearch`.

Perform the following operations : 

1. Create an index with pp_index and note down the number of primary/replica shards created by default.
2. Insert some data into the index by creating 20 to 30 documents. 
3. Read the data from the indice and write the same to a json file. [file name : read_data.json]
4. Capture the elasticsearch cluster health along with a timestamp and write it to file. [file name : cluster_health_before_step5.json]
5. Stop two data nodes from the cluster and ensure you are still able to read the same data from es and write it to a json file. [file name : read_data_after_step5.json]
6. Capture the elasticsearch cluster health along with a timestamp and write it to file. [file name : cluster_health_after_step5.json]
7. Add the nodes back to the cluster.
8. Increase replica shard count to 3 (for each primary shard you need to have 3 replicas) and capture the location of primary and replica shards and create cluster structure diagram. (Diagram should be converted to image format)
- - - - - 
Subtask for elasticsearch : 
Perform a backup of data stored in elasticsearch cluster , delete the data on live cluster , restore the data back using backup files.

Task 2 :
Server Host : stg-glusterfsintern001.phonepe.nb6
Volume : sre_interns
Install gluster-client on a machine. 

Write a script to perform the following : 

1. Create a local directory on the client machine and mount the path to the glusterfs server provided above.

2. Upload all the files generated from above `task 1`to the storage pool by creating a directory of name `your_name_intern` using the client.

3. Perform search operation on elasticsearch index and upload the results to the storage pool using the client. (Search should be using a pattern of string or word)
