
## Prerequisites

### Subscribe to the Speech Recognition API, and get a free trial subscription key

The Speech API is part of Cognitive Services. You can get free trial subscription keys from the [Cognitive Services subscription](https://azure.microsoft.com/try/cognitive-services/) page. After you select the Speech API, select **Get API Key** to get the key. It returns a primary and secondary key. Both keys are tied to the same quota, so you can use either key.

**Note:** Before you can use Speech client libraries, you must have a [subscription key](https://azure.microsoft.com/try/cognitive-services/).

## Get started

In this section we will walk you through the necessary steps to load a sample HTML page. The sample is located in our [github repository](https://github.com/Azure-Samples/SpeechToText-WebSockets-Javascript). You can **open the sample directly** from the repository, or **open the sample from a local copy** of the repository. 

**Note:** Some browsers block microphone access on un-secure origin. So, it is recommended to host the 'sample'/'your app' on https to get it working on all supported browsers. 

### Open the sample directly

Acquire a subscription key as described above. Then open the [link to the sample](https://htmlpreview.github.io/?https://github.com/Azure-Samples/SpeechToText-WebSockets-Javascript/blob/preview/samples/browser/Sample.html). This will load the page into your default browser (Rendered using [htmlPreview](https://github.com/htmlpreview/htmlpreview.github.com)).

### Open the sample from a local copy

To try the sample locally, clone this repository:

```
git clone https://github.com/Azure-Samples/SpeechToText-WebSockets-Javascript
```

compile the TypeScript sources and bundle/browserfy them into a single JavaScript file ([npm](https://www.npmjs.com/) needs to be installed on your machine). Change into the root of the cloned repository and run the commands:

```
cd Copilot && npm run bundle
```

Open `samples\browser\index.html` in your favorite browser.


## Docs
The SDK is a reference implementation for the speech websocket protocol. Check the [API reference](https://docs.microsoft.com/en-us/azure/cognitive-services/speech/API-reference-rest/bingvoicerecognition#websocket) and [Websocket protocol reference](https://docs.microsoft.com/en-us/azure/cognitive-services/speech/API-reference-rest/websocketprotocol) for more details.

## Browser support
The SDK depends on WebRTC APIs to get access to the microphone and read the audio stream. Most of todays browsers(Edge/Chrome/Firefox) support this. For more details about supported browsers refer to [navigator.getUserMedia#BrowserCompatibility](https://developer.mozilla.org/en-US/docs/Web/API/Navigator/getUserMedia#Browser_compatibility)

**Note:** The SDK currently depends on [navigator.getUserMedia](https://developer.mozilla.org/en-US/docs/Web/API/Navigator/getUserMedia#Browser_compatibility) API. However this API is in process of being dropped as browsers are moving towards newer [MediaDevices.getUserMedia](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia) instead. The SDK will add support to the newer API soon.

## Contributing
This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
