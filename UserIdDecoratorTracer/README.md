
# README

UserIDDecoratorTracer is a fully functional extension for CA APM .NET Agent to get and display user information in the Transaction Trace ("TT") TypeViewer and trace info.

Reflection is used to call one of two methods to grab the user identity from your ASP.NET application: Request cookie or NTLM authenticated user.

To use, place the extension (DLL) in your agent's EXT directory and your ProbeBuilder Directive (PBD) in your HOTDEPLOY directory. Then restart IIS.

Additional details are available in the RELEASENOTES and on the [CA APM Developer Community](http://bit.ly/caapm_dev/).
