### <a name="remove-ssl3-from-the-wcf-transportdefaults"></a>Entfernen von „Ssl3“ aus der WCF-Klasse „TransportDefaults“

|   |   |
|---|---|
|Details|Bei der Verwendung von NetTcp im Transportsicherheitsmodus und der Einstellung „Zertifikat“ wird das SSL3-Protokoll nicht mehr als eins der Standardprotokolle für das Aushandeln einer sicheren Verbindung verwendet. In den meisten Fällen sollte es keine Auswirkungen auf vorhandene Apps geben, da TLS 1.0 schon immer in der Protokollliste für „NetTcp“ enthalten ist. Alle vorhandenen Clients sollten in der Lage sein, eine Verbindung mit mindestens TLS 1.0 auszuhandeln.|
|Vorschlag|Wenn Ssl3 erforderlich ist, verwenden Sie eine der folgenden Konfigurationsmechanismen, um Ssl3 der Liste der ausgehandelten Protokolle hinzuzufügen.<ul><li><xref:System.ServiceModel.Channels.SslStreamSecurityBindingElement.SslProtocols></li><li><xref:System.ServiceModel.TcpTransportSecurity.SslProtocols></li><li>[<](~/docs/framework/configure-apps/file-schema/wcf/transport-of-nettcpbinding.md)</li><li>[&lt;sslStreamSecurity&gt; section of &lt;customBinding&gt;]~/docs/framework/configure-apps/file-schema/wcf/sslstreamsecurity.md)</li></ul>|
|Bereich|Edge|
|Version|4.6.2|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.ServiceModel.Channels.SslStreamSecurityBindingElement.SslProtocols?displayProperty=nameWithType></li><li><xref:System.ServiceModel.TcpTransportSecurity.SslProtocols?displayProperty=nameWithType></li></ul>|

