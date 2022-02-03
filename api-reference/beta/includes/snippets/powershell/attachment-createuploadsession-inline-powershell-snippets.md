---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d091ff3190ca327fc8403f5516206574a9b61775
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340368"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AttachmentItem = @{
        AttachmentType = "file"
        Name = "scenary"
        Size = 7208534
        IsInline = $true
        ContentId = "my_inline_picture"
    }
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachmentUploadSession -UserId $userId -MessageId $messageId -BodyParameter $params

```