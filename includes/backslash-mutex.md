---
ms.openlocfilehash: c28e3f97e02079905d591a7f27dc8d68d603c0bf
ms.sourcegitcommit: 5ef0d02cb57c7153fd9d5417cdcad45665af832e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/29/2019
ms.locfileid: "71140399"
---
Der umgekehrte Schrägstrich \\ stellt in Mutex-Namen ein reserviertes Zeichen dar. Verwenden Sie umgekehrte Schrägstriche (\\) in Mutex-Namen nur wie in dem Hinweis zur Verwendung von Mutex-Objekten in Sitzungen des Terminalservers beschrieben. Andernfalls kann sogar eine <xref:System.IO.DirectoryNotFoundException> ausgelöst werden, wenn der Mutex-Name für eine bereits vorhandene Datei steht.
