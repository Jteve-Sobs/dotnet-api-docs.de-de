### <a name="webutilityhtmldecode-no-longer-decodes-invalid-input-sequences"></a>WebUtility.HtmlDecode decodiert mehr ungültige Eingabesequenzen.

|   |   |
|---|---|
|Details|Decodierungsmethoden decodieren nicht mehr standardmäßig ungültige Eingabesequenzen in ungültige UTF-16-Zeichenfolgen. Stattdessen geben sie die ursprüngliche Eingabe zurück.|
|Vorschlag|Die Änderung der Decoderausgabe sollte nur von Bedeutung sein, wenn Sie Binärdaten statt der UTF-16-Daten in Zeichenfolgen speichern. Um dieses Verhalten explizit zu steuern, legen die <code>aspnet:AllowRelaxedUnicodeDecoding</code> Attribut des der ["appSettings"](~/docs/framework/configure-apps/file-schema/appsettings/index.md) Element <code>true</code> um Legacyverhalten zu aktivieren oder zu <code>false</code> auf das aktuelle Verhalten zu aktivieren.|
|Bereich|Gering|
|Version|4.5|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.Net.WebUtility.HtmlDecode(System.String)?displayProperty=nameWithType></li><li><xref:System.Net.WebUtility.HtmlDecode(System.String,System.IO.TextWriter)?displayProperty=nameWithType></li><li><xref:System.Net.WebUtility.UrlDecode(System.String)?displayProperty=nameWithType></li></ul>|

