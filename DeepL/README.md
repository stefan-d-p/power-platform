# DeepL Translate Connector
DeepL is an online service and API for translating text and documents into more than 25 languages.

# Prerequisites

* A Microsoft Power Apps or Power Automate plan with custom connector feature
* A [DeepL](https://www.deepl.com) API account (free tier available)

# Operations

### TranslateText

Translates plain text, xml and html.

### TranslateDocumentRequest

Sends a Microsoft Office or PDF document to DeepL for translation. Translating documents is an asynchronous operation. After you have uploaded the document using this operation you have to periodically check the translation status

### CheckDocumentTranslationStatus

Checks the translation status for a document upload. Returns one of the following status

* Translating - The document is currently translated
* Done - Translation is finished and translated document is ready to download
* Error - An error has occured during translation

### DownladDocument

Downloads a translated document once translation has finished

### GetLanguages

Retrieves supported languages by DeepL, either used as source language or target language. This operation is also used to dynamically populate the input parameters for TranslateText and TranslateDocumentRequest.
