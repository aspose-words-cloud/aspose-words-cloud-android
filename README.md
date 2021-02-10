![](https://img.shields.io/badge/api-v4.0-lightgrey) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/aspose-words-cloud/aspose-words-cloud-java) [![GitHub license](https://img.shields.io/github/license/aspose-words-cloud/aspose-words-cloud-java)](https://github.com/aspose-words-cloud/aspose-words-cloud-java)


# Android SDK for Word Documents Processing in the Cloud
[Aspose.Words Cloud Java SDK for Android](https://products.aspose.cloud/words/android) allows to work with Word document headers, footers, page numbering, tables, sections, document comments, drawing objects, FormFields, fonts, hyperlinks, ranges, paragraphs, math objects, watermarks, revisions and document protection. It also assists in appending documents, splitting documents as well as converting document to other supported file formats. Please feel free to explore the [Developer's Guide](https://docs.aspose.cloud/display/wordscloud/Developer+Guide) for all possible usage scenarios.
Feel free to explore the [Developer's Guide](https://docs.aspose.cloud/display/wordscloud/Developer+Guide) & [API Reference](https://apireference.aspose.cloud/words/) to know all about Aspose.Words Cloud API.

## Document Processing Services in REST

- Convert between various document-related formats, including Word to PDF & vice versa.
- Mail merge and report generation in the Cloud.
- Split & merge Word documents.
- Access Word document metadata.
- Find and replace text.
- Add & remove watermarks and protection.
- Read & write access to Document Object Model.
- Get document information in JSON or XML representation.
- Convert an encrypted PDF document into Word document format.
- [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
- [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
- [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.

Check out the [Developer's Guide](https://docs.aspose.cloud/display/wordscloud/Developer+Guide) to know more about Aspose Words Cloud REST API.


## Read & Write Document Formats

**Microsoft Word:** DOC, DOCX, RTF, DOT, DOTX, DOTM, FlatOPC (XML)
**OpenOffice:** ODT, OTT
**WordprocessingML:** XML
**Web:** HTML, MHTML, HtmlFixed
**Text:** TXT
**Fixed Layout:** PDF

## Save Document As

**Fixed Layout:** PDF/A, XPS, OpenXPS, PS
**Images:** JPEG, PNG, BMP, SVG, TIFF, EMF
**Others:** PCL

## Enhancements in Version 21.1

- Added the typed `NodePath` builder.
- Added online version for all API methods.
- During the conversion process the invisible text from `PDF` will be skipped now.
- Improved the font style recognition for the Hebrew language pages.


## Enhancements in Version 20.11
- In configuration json file appSid / appKey has been replaced to clientId / clientSecret.
- In Words API initialization methods clientId parameter precedes clientSecret parameter.

## Enhancements in Version 20.10
- Internal API changes.

## Enhancements in Version 20.9
- Added Batch API feature


### Prerequisites

To use Aspose Words Cloud SDK for Java you need to register an account with [Aspose Cloud](https://www.aspose.cloud/) and lookup/create App Key and SID at [Cloud Dashboard](https://dashboard.aspose.cloud/#/apps). There is free quota available. For more details, see [Aspose Cloud Pricing](https://purchase.aspose.cloud/pricing).

## Dependencies
- Java 1.7+
- referenced packages (see [here](https://github.com/rizwanniazigroupdocs/aspose-words-cloud-java/blob/master/pom.xml) for more details)

## Licensing

All Aspose.Words Cloud SDKs, helper scripts and templates are licensed under [MIT License](https://github.com/aspose-words-cloud/aspose-words-cloud-java/blob/master/LICENSE).

## Contact Us
Your feedback is very important to us. Please feel free to contact us using our [Support Forums](https://forum.aspose.cloud/c/words).

## Getting Started
1. **Sign Up**. Before you begin, you need to sign up for an account on our [Dashboard](https://dashboard.aspose.cloud/) and retrieve your [credentials](https://dashboard.aspose.cloud/#/apps).
2. **Minimum requirements**. This SDK requires [Java 1.7 or later](https://java.com/download/).
3. **Add Aspose.Words Cloud SDK for Java to your project**. The project in this repo references [Aspose.Words Cloud SDK for Java](https://github.com/aspose-words-cloud/aspose-words-cloud-java) either by placing the binary inside *app/libs* folder with manual handling of transitive dependenices (meant for internal usage only), or by simple addition of the repository dependency with configuring the project accordingly (user scenario) - the behavior is controlled with *CI* environment variable (see [build.gradle](app/build.gradle)). For the users, the following basic instructions should be applied.

Since this library is consuming Aspose.Words Cloud web APIs, please add *INTERNET* permission to your manifest.

## Delete Watermark from Document in Android using Java

```java
	// Get your ClientId and ClientSecret from https://dashboard.aspose.cloud (free registration required).
	WordsApi wordsApi = new WordsApi("MY_CLIENT_ID", "MY_CLIENT_SECRET", "api.aspose.cloud");

	String localPath = PathUtil.get(localFolder, fileName);
	String remotePath = PathUtil.get(remoteFolder, remoteName);

	UploadFileRequest uploadRequest = new UploadFileRequest(Files.readAllBytes(Paths.get(localPath)), remotePath, null);
	//wordsApi.uploadFile(uploadRequest);

	DeleteWatermarkRequest request = new DeleteWatermarkRequest(remoteName, remoteFolder, null, null, null, null, null, null);
	DocumentResponse result = wordsApi.deleteWatermark(request);

```

## Aspose.Words Cloud SDKs in Popular Languages

| .NET | Java | PHP | Python | Ruby | Node.js | Android | Swift|Dart|Go|
|---|---|---|---|---|---|---|--|--|--|
| [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-dotnet) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-java) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-php) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-python) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-ruby)  | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-node) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-android) | [GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-swift)|[GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-dart) |[GitHub](https://github.com/aspose-words-cloud/aspose-words-cloud-go) |
| [NuGet](https://www.nuget.org/packages/Aspose.Words-Cloud/) | [Maven](https://repository.aspose.cloud/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words-cloud) | [Composer](https://packagist.org/packages/aspose-cloud/aspose-words-cloud) | [PIP](https://pypi.org/project/aspose.words-cloud/) | [GEM](https://rubygems.org/gems/aspose_words_cloud)  | [NPM](https://www.npmjs.com/package/asposewordscloud) | [Maven](https://repository.aspose.cloud/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-words-cloud) | [Cocoapods](https://cocoapods.org/pods/AsposeWordsCloud)|[Pub.Dev](https://pub.dev/packages/aspose_words_cloud) | [Go.Dev](https://pkg.go.dev/github.com/aspose-words-cloud/aspose-words-cloud-go/) |

[Product Page](https://products.aspose.cloud/words/android) | [Documentation](https://docs.aspose.cloud/display/wordscloud/Home) | [API Reference](https://apireference.aspose.cloud/words/) | [Code Samples](https://github.com/aspose-words-cloud/aspose-words-cloud-dotnet) | [Blog](https://blog.aspose.cloud/category/words/) | [Free Support](https://forum.aspose.cloud/c/words) | [Free Trial](https://dashboard.aspose.cloud/#/apps)
