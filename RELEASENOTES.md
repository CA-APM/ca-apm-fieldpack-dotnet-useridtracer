# CA APM FIELDPACK .NET User ID Decorator Tracer

1. [DESCRIPTION](#description)
1. [INSTALLATION](#installation)
1. [CONFIGURATION](#configuration)
1. [TROUBLESHOOTING](#troubleshooting)
1. [CHANGELOG](#changes)

## <a name="description"></a>DESCRIPTION

The .NET Agent User ID Decorator Tracer sole purpose is display the user's domain credentials in the Transaction Trace TypeViewer and in the stack trace details.
The tracer is called by a directive in custom ProbeBuilder Directive (PBD), which in turn "decorates" the requests and adds the user credentials to the stack trace.

Discussions about the use or enhancement of the FieldPack will be found on the [CA APM Developer Community](http://bit.ly/caapm_dev/). Each artifact may have its own README or RELEASENOTES to explain the asset.

## <a name="installation"></a>INSTALLATION

To deploy the extension, place the assembly in the agent's EXT directory; the PBD can either go into HOTDEPLOY (recommended) or with the default directives in the WILY directory.
If you choose the latter, you will need to modify IntroscopeAgent.profile to include the PBD in your 'directivesFile' property.
Restart IIS when the installation's complete.

## <a name="configuration"></a>CONFIGURATION

If for any reason you need to modify how and when the tracer is called, do this via userIdtracer.pbd.
Do NOT alter the directive "SetTracerClassMapping"!

## <a name="troubleshooting"></a>troubleshooting

Locate and edit logging.xml.
Change the logging level from INFO to DEBUG, then save.
If you do not see DEBUG statements in the agent's log within a few seconds of the change, please restart IIS.

## <a name="changes"></a>CHANGELOG

Please review the **CHANGELOG.md** file in this repository

## <a name="license"></a>LICENSE

Please review the **LICENSE** file in this repository.

