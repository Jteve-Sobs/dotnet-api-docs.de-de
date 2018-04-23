### <a name="wpf-datatemplate-elements-are-now-visible-to-uia"></a>WPF DataTemplate-Elemente sind jetzt für die UIA sichtbar

|   |   |
|---|---|
|Details|In der Vergangenheit waren <xref:System.Windows.DataTemplate?displayProperty=name>-Elemente für die Benutzeroberflächenautomatisierung nicht sichtbar. Ab Version 4.5 erkennt die Benutzeroberflächenautomatisierung diese Elemente. Dies ist zwar in vielen Fällen hilfreich, kann aber bei Tests zu Problemen führen, die von UIA-Strukturen abhängen, die keine <xref:System.Windows.DataTemplate?displayProperty=name>-Elemente enthalten.|
|Vorschlag|Tests für die Benutzeroberflächenautomatisierung für diese App müssen möglicherweise aktualisiert werden, um die UIA-Struktur zu berücksichtigen, die jetzt zuvor unsichtbare <xref:System.Windows.DataTemplate?displayProperty=name>-Elemente enthält. Beispielsweise müssen Tests, die erwarten, dass einige Elemente nebeneinander angeordnet sind, jetzt möglicherweise davon ausgehen, dass sich zwischen diesen Elementen zuvor unsichtbare UIA-Elemente befinden. Möglicherweise müssen auch Tests mit neuen Werten aktualisiert werden, die auf bestimmte Werte oder Indizes für UIA-Elemente angewiesen sind.|
|Bereich|Edge|
|Version|4.5|
|Typ|Laufzeit|
|Betroffene APIs|<ul><li><xref:System.Windows.DataTemplate.%23ctor?displayProperty=nameWithType></li><li><xref:System.Windows.DataTemplate.%23ctor(System.Object)?displayProperty=nameWithType></li></ul>|

