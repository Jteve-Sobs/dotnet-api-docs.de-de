### <a name="appdomainsetupdynamicbase-is-no-longer-randomized-by-userandomizedstringhashalgorithm"></a>AppDomainSetup.DynamicBase wird mithilfe von UseRandomizedStringHashAlgorithm nicht mehr zufällig festgelegt

|   |   |
|---|---|
|Details|Vor .NET Framework 4.6 wurde der Wert von <xref:System.AppDomainSetup.DynamicBase> für Anwendungsdomänen oder Prozesse zufällig festgelegt, wenn UseRandomizedStringHashAlgorithm in der Konfigurationsdatei der App aktiviert war. Ab .NET Framework 4.6 gibt <xref:System.AppDomainSetup.DynamicBase> ein stabiles Ergebnis zurück, das zwischen verschiedenen Instanzen einer ausgeführten App und zwischen verschiedenen App-Domänen besteht. Verschiedene Apps haben auch unterschiedliche dynamische Basen. Diese Änderung entfernt nur die Elemente von verschiedenen Instanzen einer App, die zufällig benannt werden.|
|Vorschlag|Beachten Sie, dass bei der Aktivierung von <code>UseRandomizedStringHashAlgorithm</code> <xref:System.AppDomainSetup.DynamicBase> nicht zufällig festgelegt wird. Wenn eine zufällige Basis benötigt wird, muss diese im Code Ihrer App anstelle einer API erstellt werden.|
|Bereich|Edge|
|Version|4.6|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.AppDomainSetup.DynamicBase?displayProperty=nameWithType></li></ul>|

