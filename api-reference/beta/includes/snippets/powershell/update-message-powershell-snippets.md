---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b59172657d75a9092bd6cc2d51ed96b85cc6f0f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351352"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    InferenceClassification = "other"
}

# A UPN can also be used as -UserId.
Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```