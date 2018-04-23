### <a name="log-file-name-created-by-the-objectcontextcreatedatabase-method-has-changed-to-match-sql-server-specifications"></a>Der von der ObjectContext.CreateDatabase-Methode erstellte Protokolldateiname wurde geändert, um den SQL Server-Spezifikationen zu entsprechen

|   |   |
|---|---|
|Details|Wenn die <xref:System.Data.Objects.ObjectContext.CreateDatabase?displayProperty=name>-Methode entweder direkt oder durch Code First mit dem SqlClient-Anbieter und einem AttachDBFilename-Wert in der Verbindungszeichenfolge aufgerufen wird, erstellt sie eine Protokolldatei namens „Dateiname_log.ldf“ anstelle von „Dateiname.ldf“ (wobei „Dateiname“ der vom AttachDBFilename-Wert angegebene Name der Datei ist). Diese Änderung verbessert das Debuggen, indem eine Protokolldatei bereitgestellt wird, die nach den SQL Server-Spezifikationen benannt wird.|
|Vorschlag|Wenn der Name der Protokolldatei für eine App wichtig ist, sollte die App aktualisiert werden, um das standardmäßige Dateinamenformat „_log.ldf“ zu erwarten.|
|Bereich|Edge|
|Version|4.5|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.Data.Objects.ObjectContext.CreateDatabase?displayProperty=nameWithType></li></ul>|

