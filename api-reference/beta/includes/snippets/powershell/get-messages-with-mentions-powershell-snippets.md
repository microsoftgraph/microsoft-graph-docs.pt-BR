---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23b08d9122917e6a5b55321d7d0d1df857c241f2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352165"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -Filter "MentionsPreview/IsMentioned eq true" -Property "Subject,Sender,ReceivedDateTime,MentionsPreview" 

```