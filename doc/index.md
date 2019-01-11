# Create the Azure Search Index via REST

We will create the schema of our Azure Search Index.

Create the post request:

- The api-version will be provided as Parameter. The URL will look like this - make sure to replace `mySearchService` with your Instance name.

    https:/`mySearchService`.search.windows.net/indexes?api-version=`2017-11-11-Preview`
- The api-key will be provided as Header. 
- The request body is defined in `index.json`

  Postman Post Request: 
   ![](img/create_index.jpg)
   ![](img/create_index_2.jpg)