---
ms.openlocfilehash: b43d88a9e48278469fdc0c0d3422e91ae04dde28
ms.sourcegitcommit: 11d168140aa8fade0768c2a9dde3e3bcacfdfb7d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/27/2020
ms.locfileid: "83888166"
---

Wenn jedoch die **String.Format**-Methode aufgerufen wird, müssen Sie sich nicht auf die genaue Überladung konzentrieren, die Sie aufrufen möchten. Stattdessen können Sie die Methode mit einer [kombinierten Formatzeichenfolge](/dotnet/standard/base-types/composite-formatting) aufrufen, die mindestens ein Formatelement enthält. Weisen Sie jedem Formatelement einen numerischen Index zu. Der erste Index startet bei 0 (null). Neben dem ersten Zeichenfolgenwert sollte Ihr Methodenaufruf über gleich viele zusätzliche Argumente und Indexwerte verfügen. Beispielsweise sollte eine Zeichenfolge, deren Formatelemente die Indizes 0 und 1 aufweisen, über zwei Argumente verfügen. Dabei sollte ein Argument über bis zu fünf Indizes und eins über sechs Argumente verfügen. Ihr Sprachcompiler ruft dann einen Methodenaufruf einer bestimmten Überladung der **String.Format**-Methode auf.   
 
Weitere Informationen zur **String.Format**-Methode finden Sie unter [Getting started with the String.Format method (Erste Schritte mit der String.Format-Methode)](#Starting) und [Which method do I call? (Welche Methode soll ich aufrufen?)](#FTaskList).    
