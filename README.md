# webex-calling-api-examples
This repo provides Postman collections that demonstrates the use of the [Webex Calling API](https://developer.webex.com/docs/api/guides/webex-calling).

To exercise these API simply do the following
* [Install Postman](https://www.postman.com/downloads/)
* [Import the collection](#import-the-collection)
* [Configure the environment](#configure-the-environment)
* [Exercise the requests](#exercise-the-resquests)

## Import the collection
1) Clone this repo or simply download the [postman collection](./webex-calling-calls-api.json) to your local disk.
2) From within Postman , begin by clicking the "Import" button, and choosing the "Choose Files" button:

  ![Postman Import](./images/import.png)

Select the collection in any sub-folder that you wish import. When imported successfully you should see new collection in postman.

## Configure the Environment

This collection uses "collection level" variables, which simply means that you can specify an environment that is unique to you, directly from within the collection itself.   

Each collection in this repo's sub-folders have different environment variables. Refer to individual sub-folders for description of these environment variables. 

To edit the variables first click on the "three dots" associated with the collection and select edit

  ![Edit Collection](./images/edit-collection.png)

Then click on the "Variables" tab and update the values in the "Current Value" column as you need to:

  ![Set Variables](./images/set-variables.png)

If you are familiar with Postman's environments, its worth noting that you don't need to explicitly set an environment to run these requests, since all the variables are set at the collection level.  If you do have an active environment that sets any of the environment variables used by this collection, the active environment variables will take precedence. 

Click the update button, and you are ready to try the requests.

## Exercise the requests

After sending the request scroll down to see the response.  The "Test Results" section will provide information on which tests passed (or failed).

  ![Response](./images/response.png)

Inspect the request and response to better understand how the API works and move on to the next request in the folder.

Have fun!
