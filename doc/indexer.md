# Create the Azure Search Indexer via REST

The Azure Search Indexer defines the pipeline and connects the Index, Data source and used Skillsets.

Create the post request:

- The api-version will be provided as Parameter. The URL will look like this - make sure to replace `mySearchService` with your Instance name.

    https:/`mySearchService`.search.windows.net/indexer?api-version=`2017-11-11-Preview`
- The api-key will be provided as Header. 
- The request body is defined in `indexer.json`

  Post request: 
     ![](img/create_indexer.jpg)