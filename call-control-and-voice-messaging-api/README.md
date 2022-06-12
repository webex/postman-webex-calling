# webex-calling-calls-apis

* [Configure the environment](#configure-the-environment)
* [Exercise the requests](#exercise-the-resquests)

## Configure the Environment

The environment variables for the collection in this folder:

* WEBEX_TOKEN -- an OAuth token for a user configured for calling in the test environment. These tests require a token with all the calling scopes (spark:calls_read and spark:calls_write).  To get started quickly, developers can copy their temporary token from the [Webex For Developers Gettings Started Guide](https://developer.webex.com/docs/api/getting-started#accounts-and-authentication). 
* WEBEX_API_URL -- the URL of the API under test, generally the default value of "https://webexapis.com/v1/" does not need to be changed
* DESTINATION -- The destination to be dialed. Destination can be extensions, PSTN numbers, FAC codes or SIP URI. The destination can be digits or a URI. Some examples for destination include: 1234, 2223334444, +12223334444, *73, tel:+12223334444, user@company.domain, sip:user@company.domain
* TRANSFER_DESTINATION -- The destination to be dialed. This is used to make a second call from the api user in order to transfer the call.
* PARK_DESTINATION  -- The destination to park the call.
* VOICE_MESSAGE_ID  -- The message Id for Voice Message APIs that require an Id for the action.

## Exercise the requests

The collection consists of five folders that exercise the following use cases:

1) Create an outbound (Click to Dial) Call and verify it is gettable and perform a basic Hold and Resume operation on the call.
2) Answer an inbound call (UserA calls apiUser), initiate another call from the same user (apiUser calls UserB) and perform a Consult Transfer (i.e. apiUser transfers the call to connect UserA with UserB)
3) Answer an inbound call (UserA calls apiUser) and blind transfer (Divert) the call to apiUser's voicemail.
4) Answer an inbound call, park the call on another destination and retrieve the call back to apiUser.
5) Answer an inbound call, start recording, the pause recording, resume recording and stop call recording and then end the call.
**Note:** The apiUser must be enabled for Call Recording in Control Hub and should have "On Demand" Call Recording option selected. Also, the apiUser information must be provisioned the Dubber account (i.e. user and dub point should be created prior to using these APIs)
6) Get Call History (i.e. missed calls, placed calls and received calls).
7) Voice Messages (example usage of the voice message APIs).

Each folder is standalone, but the requests are meant to be run one after the other.

The last request in each folder will run a pre-request script that will "clean up" the temporary environment variables that were set and used in the pre-request and test script.
