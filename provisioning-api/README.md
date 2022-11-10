# webex-calling-provisioning-apis

## Configure the Environment

The environment variables for the collection in this folder:

* WEBEX_TOKEN -- OAuth token with appropriate calling scopes. To get started quickly, developers can copy their temporary token from the [Webex For Developers Gettings Started Guide](https://developer.webex.com/docs/api/getting-started#accounts-and-authentication). 
* WEBEX_API_URL -- The URL of the API under test, generally the default value of "https://webexapis.com/v1/" does not need to be changed.
* LOCATION_ID -- The location id for location feature APIs that require an id for the action.
* PERSON_ID -- The person id for person feature APIs that require an id for the action.
* MONITORED_AGENTID_1 -- The person/place id used by person feature APIs for being monitored.
* MONITORED_AGENTID_2 -- The person/place id used by person feature APIs for being monitored.
* SCHEDULE_TYPE -- Valid schedule type used by person feature schedule and event APIs.
* WORKSPACE_ID -- Valid workspaceId used by the numbers feature for a workspace
* LOCATIONID_FOR_DEVICES -- Valid locationId to which all configured devices belong.
* MAC_ADDRESS -- The input MAC addresses that needs to be validated.
* DEVICE_MODEL -- Model name of the device for which settings needs to be retrieved.
* DEVICE_ID -- Valid device id to fetch/update current configuration settings.
* APPLICATION_ID -- Valid application id.
