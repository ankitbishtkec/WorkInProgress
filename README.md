# WorkInProgress
These are two project( Flipkart's Aesop and Flipkart's Open Replicator) I am working on and will opensource the changes once done.

# Changes already done:
# FK's Aesop:
1. Editing Kafka data layer to insert data in JSON instead of pre-programmed AVRO schema.
2. Getting Old and new mysql row values on upsert( update or insert).

# FK's Open replicator:
1. Made Open replicator fault tolerant for MySQL restart events.
2. Making sure it continues from last read MySQL bin-logs on retrying after crash instead of retrying from beginning.

#Deployment:
Another contributor has added ansible to deploy a working cluster of AESOP, Zookeeper and kafka.

#TODO:
1. Add Spring file config code to allow Aesop relay server to read from multiple MySQL DBs and allow aesop client servers to read from multiple relay servers. Current configuration allows single db read for relay and single relay read for client. 
2.Take Flipkart's Aesop and Flipkart's Open Replicator fork merge own changes and raise request to pull the changes.

