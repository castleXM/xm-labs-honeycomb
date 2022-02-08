# honeycomb.io

This integration allows you to alert users in xMatters after an alert goes off in [honeycomb.io](https://honeycomb.io).


---------

<kbd>
<a href="https://support.xmatters.com/hc/en-us/community/topics">
   <img src="https://github.com/xmatters/xMatters-Labs/raw/master/media/disclaimer.png">
</a>
</kbd>

---------

An updated version of this integration is available. You can install the new version right from the Workflow Templates directory within your xMatters instance. [Learn more](http://help.xmatters.com/integrations/#cshid=Honeycomb).

---------

# Files

* [honeycombio.zip](honeycombio.zip) - Workflow zip file with the step and example flow
* [honeycomb.png](/honeycomb.png) - honeycomb.io logo

# How it works
This integration uses an HTTP recipient from a honeycomb.io trigger and creates an xMatters alert from it.


# Installation

## xMatters Setup
1. Download the [honeycombio.zip](honeycombio.zip) file onto your local computer
2. Navigate to the Workflows tab of your xMatters instance
3. Click Import, and select the zip file you just downloaded
4. In the **Create Event** step of the **Alert** flow, select the recipients for the alert.
5. Open the HTTP trigger on the left side of the flow and copy the URL for use in honeycomb.io.


## honeycomb.io Setup
You'll need to create and attach a Webhook recipient to a trigger in honeycomb.io.

1. Start to create a trigger in honeycomb.io
2. On the recipients section, click the link to the Integration Center.
3. Click the **Add Integration** button.
    1. Select **Webhook** as the provider.
    2. Name it whatever you like, we recommend just calling it **xMatters**
    3. Take the link you got from the HTTP trigger in xMatters and paste it under **Webhook URL**
    4. The value for shared secret does not matter.
4. Add the newly created recipient in the Trigger.


## Example
This is an image of the provided flow.

<kbd>
	<img src="/media/ExampleFlow.png">
</kbd>

