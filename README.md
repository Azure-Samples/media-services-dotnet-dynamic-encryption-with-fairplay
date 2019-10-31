---
page_type: sample
languages:
- csharp
products:
- azure
description: "Azure Media Services enables your to dynamically encrypt your HTTP Live Streaming (HLS) content using Apple FairPlay."
urlFragment: media-services-dotnet-dynamic-encryption-with-fairplay
---

# Stream your HLS content Protected with Apple FairPlay using Azure Media Services v2 

Azure Media Services enables your to dynamically encrypt your HTTP Live Streaming (HLS) content using Apple FairPlay. When encrypting with FairPlay, individual video and audio samples are encrypted using the AES-128 CBC mode. FairPlay Streaming (FPS) is integrated into the device operating systems, with native support on iOS and Apple TV. Safari on OS X enables FPS using Encrypted Media Extensions (EME) interface support.

This sample shows you how to configure Azure Media Services to stream your content protected with FairPlay. It also shows how to specify to deliver the FairPlay licenses to your clients. 

For detailed description of this sample, see [this](https://azure.microsoft.com/en-us/documentation/articles/media-services-protect-hls-with-fairplay/) article.

## How To Run This Sample

To run this sample you will need:

- Visual Studio  
- An Azure subscription
- Latest Azure Media Services .NET SDK (which will be installed when you re-build the project).

### Step 1:  Clone or download this repository

### Step 2: Update the app.config file

Update the appSettings section of the app.config file with appropriate values. For more information, see [this](https://docs.microsoft.com/azure/media-services/media-services-use-aad-auth-to-access-ams-api) topic.

	<appSettings>
		<add key="AMSAADTenantDomain" value="tenant"/>
		<add key="AMSRESTAPIEndpoint" value="endpoint"/>
		<add key="AMSClientId" value="id"/>
		<add key="AMSClientSecret" value="secret"/>

		<add key="Issuer" value="http://testacs.com" />
		<add key="Audience" value="urn:test" />
	</appSettings>

### Step 3: Start a streaming endpoint

Make sure to start the streaming endpoint. For more information, see: [streaming endpoints](https://docs.microsoft.com/azure/media-services/media-services-portal-manage-streaming-endpoints).

### Step 4:  Run the sample

Clean the solution, rebuild the solution, and run it. 


## About the code

For more information, see  [Use Azure Media Services to Stream your HLS content Protected with Apple FairPlay](https://azure.microsoft.com/en-us/documentation/articles/media-services-protect-hls-with-fairplay/).

## More information

You can view AMS learning paths here:

- [AMS Live Streaming Workflow](http://azure.microsoft.com/documentation/learning-paths/media-services-streaming-live/)
- [AMS on Demand Streaming Workflow](http://azure.microsoft.com/documentation/learning-paths/media-services-streaming-on-demand/)
