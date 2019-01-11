# Create the Blob Storage 
 
 The blob will be used as input source for the Indexer.

 1) Create a Storage account in the Azure portal using the defaults
 2) Select Blobs and create a container `txdata`. Use the defaults
 3)  Select the container and Upload the `tx.json` which contains sample input data
 4) Get the `connectionString` to access the blob:
    >Azure Portal : _Storage account > Settings > Access Keys > Connection string_

    Update the value `connectionString` in `datasource.json`.
