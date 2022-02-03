---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad8e8be83975be1814f08f78c2d6efc48d7683f2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350144"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Remove-MgUserEventAttachment -UserId $userId -EventId $eventId -AttachmentId $attachmentId

```