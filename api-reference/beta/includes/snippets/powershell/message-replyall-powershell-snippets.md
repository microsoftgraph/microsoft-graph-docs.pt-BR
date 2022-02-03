---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1be0057fd56fca16999b0ce42296576384c47c0e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341075"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.fileAttachment"
                Name = "guidelines.txt"
                ContentBytes = "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
            }
        )
    }
    Comment = "Please take a look at the attached guidelines before you decide on the name."
}

# A UPN can also be used as -UserId.
Invoke-MgReplyAllUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```