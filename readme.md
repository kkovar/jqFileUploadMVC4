# **jQFileUploadMVC4** #

This is an example of how to integrate a [jQuery-File-Upload plugin](https://github.com/blueimp/jQuery-File-Upload) into an ASP.NET MVC 4 application.

This was created as a new MVC4 ASP.net project in VS2012 using the "Basic" template. I then copied the files from jQuery_File_Upload.MVC4.Upload (in the Contents directory and the Index.cshtml) and tweaked the script includes to get it to work.

** below is from original Readme by Max.  Thanks Max.  Your work really helped me.

It is identical to the [original plugin demo](http://blueimp.github.com/jQuery-File-Upload/ "jQuery File Upload Demo") and supports batch **upload**, **download** and **deletion** of uploaded files.

Currently MVC Actions are not used to handle upload/download/delete in the demo, due to the inability for a developer to set a maxMessageLength per location in ASP.NET MVC application. IIS by default allows POST messages no londer then 5MB. This does not allow to upload large files, casting an implementation useless. Or, you can sacrifice security and just enable maxMessageLength for an entire site, which I personally wouldn't do.

This given, a HttpHandler implmentation is introduced. (thanks go to [Iain Ballard](https://github.com/i-e-b/) and his [ASP.NET handler-based demo](https://github.com/i-e-b/jQueryFileUpload.Net))

main.js is initialized with large-files in mind, and a thumbnails are smart enough to disaplay everything correctly, so go ahead, take a look and fork if you wish.