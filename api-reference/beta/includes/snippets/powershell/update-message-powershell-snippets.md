---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8053ce06530f3e7b4ff73cac0d3ac49e53cbe505
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105811"
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

Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```