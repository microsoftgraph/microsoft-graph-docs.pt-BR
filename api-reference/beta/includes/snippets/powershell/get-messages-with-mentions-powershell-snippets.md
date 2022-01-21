---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0333fdf81721358a2aad6d4b3fc4cf08f804eea7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122770"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -Filter "MentionsPreview/IsMentioned eq true" -Property "Subject,Sender,ReceivedDateTime,MentionsPreview" 

```