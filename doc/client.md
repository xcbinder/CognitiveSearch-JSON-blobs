# Create a AzSearch.js client 
 
 The AzSearch.js client is a nice option to create a customizable interface for your search.

 1) GitHub  - [AzSearch.js](https://github.com/Yahnoosh/AzSearch.js)
 2) You can use the App Generator to create the client
 3) Make sure CORS is enabled for your index:

    >Azure Portal : _mySearchService > txindex > CORS_

4) Make sure you are using a query key and not the admin key to query the index. Create a query key:

    >Azure Portal : _mySearchService > Keys > Manage query keys_

5) The App App Generator is producing the HTML. You can edit the initialize section to change connection settings if needed:

    ```javascript
    // Initialize and connect to your search service
    var automagic = new AzSearch.Automagic({ index: "txindex", queryKey: "myQueryKey", service: "mySearchService" });
    automagic.store.setSearchApiVersion("2017-11-11");
    automagic.store.setInput("Secret Project");