### <a name="calling-datagridcommitedit-from-a-celleditending-handler-drops-focus"></a>Der Aufruf von DataGrid.CommitEdit über einen CellEditEnding-Handler verliert den Fokus

|   |   |
|---|---|
|Details|Wenn das <xref:System.Windows.Controls.DataGrid.CommitEdit>-Element von einem der <xref:System.Windows.Controls.DataGrid.CellEditEnding?displayProperty=name>-Ereignishandler von <xref:System.Windows.Controls.DataGrid?displayProperty=name> aufgerufen, verliert <xref:System.Windows.Controls.DataGrid?displayProperty=name> den Fokus.|
|Vorschlag|Dieses Problem wurde in .NET Framework 4.5.2 behoben, daher kann es durch ein Upgrade von .NET Framework vermieden werden. Alternativ kann dies vermieden werden, indem das <xref:System.Windows.Controls.DataGrid?displayProperty=name>-Element nach dem Aufruf von <xref:System.Windows.Controls.DataGrid.CommitEdit?displayProperty=name> explizit neu ausgewählt wird.|
|Bereich|Edge|
|Version|4.5|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.Windows.Controls.DataGrid.CommitEdit?displayProperty=nameWithType></li><li><xref:System.Windows.Controls.DataGrid.CommitEdit(System.Windows.Controls.DataGridEditingUnit,System.Boolean)?displayProperty=nameWithType></li></ul>|

