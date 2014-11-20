#Silverlight WebClient
Silverlight's .NET WebClient does not include a number of helpful functions for making POST and GET requests simple. Using HttpWebRequest and WebRequest, these requests can still be made, but only asynchronously, causing a lot more code when you just to make a simple synchronous request. To resolve this, I created a SilverlightWebClient class with some of the missing functionality.

###DownloadData(Uri address)
Downloads the resource as a string from the URI specified.

###UploadValues(Uri address, Dictionary<string, string> data)
Uploads the specified name/value collection to the resource identified by the specified URI.