### <a name="workflow-sql-persistence-adds-primary-key-clusters-and-disallows-null-values-in-some-columns"></a>Über die SQL-Workflowpersistenz werden Primärschlüsselcluster hinzugefügt und NULL-Werte in einigen Spalten nicht zugelassen

|   |   |
|---|---|
|Details|Ab .NET Framework 4.7 verwenden die vom SqlWorkflowInstanceStoreSchema.sql-Skript erstellten Tabellen für SQL Workflow Instance Store (SWIS) Primärschlüsselcluster. Aus diesem Grund unterstützen Identitäten keine <code>null</code>-Werte. Diese Änderung hat keine Auswirkungen auf SWIS. Die Updates wurden erstellt, um die Transaktionsreplikation mit SQL Server zu unterstützen.|
|Vorschlag|Die SQL-Datei „SqlWorkflowInstanceStoreSchemaUpgrade.sql“ muss auf bereits vorgenommene Installationen angewendet werden, damit diese Änderung vorgenommen wird. Bei neuen Datenbankinstallationen werden die Änderungen automatisch vorgenommen.|
|Bereich|Edge|
|Version|4.7|
|Typ|Laufzeit|

