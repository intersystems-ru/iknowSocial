iknowSocial
===========

###General description
As for **now** `iknowSocial` provides following:
  * COS-wrapper for [VK API](http://vk.com/dev/methods).
  * Convenient way to work comfortably with VK data, using classes from `VKReader.Data` package.
  * Lister for `iKnow` to directly load/list VK data to your domain/loader.
  * Simple [demo](../master/VKReader/Viewer.xml).

###Limitations
  * `iknowSocial` only runs on Cache 2015.1 and later, due to iKnow stemming usage.

###Installation
To install `iknowSocial`, import code from this repo to your namespace with a user who has access to `%SYS` and SSL configurations editing, and run the following line in terminal:

    set status = ##class(VKReader.Utils).Install()

In case all went smooth, you'll get your status `$$$OK`.
Under the hood this method creates an empty SSL configuration with name defined by parameter `SSLConfigurationName` from class `VKReader.Requests.RequestSender`.
