### <a name="obsoleteattribute-exports-as-both-obsoleteattribute-and-deprecatedattribute-in-winmd-scenarios"></a>ObsoleteAttribute wird in WinMD-Szenarios sowohl als ObsoleteAttribute als auch als DeprecatedAttribute exportiert

|   |   |
|---|---|
|Details|Wenn Sie eine Windows-Metadatenbibliothek (WINMD-Datei) erstellen, wird das Attribut <xref:System.ObsoleteAttribute?displayProperty=name> als <xref:System.ObsoleteAttribute?displayProperty=name> und als [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute) exportiert.|
|Vorschlag|Durch die Neukompilierung von vorhandenem Quellcode, in dem das Attribut <xref:System.ObsoleteAttribute?displayProperty=name> verwendet wird, können Warnungen generiert werden, wenn dieser Code von C++/CX oder JavaScript verarbeitet wird. Es wird davon abgeraten, sowohl <xref:System.ObsoleteAttribute?displayProperty=name> als auch [Windows.Foundation.DeprecatedAttribute](https://docs.microsoft.com/uwp/api/windows.foundation.metadata.deprecatedattribute) in Code in verwalteten Assemblys anzuwenden, da dies zu Buildwarnungen führen kann.|
|Bereich|Edge|
|Version|4.5.1|
|Typ|Neuzuweisung|

