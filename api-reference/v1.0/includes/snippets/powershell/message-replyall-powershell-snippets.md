---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6382639dfdb7116c77630d6dddfc7fdd0769c255
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343246"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "comment-value"
}

# A UPN can also be used as -UserId.
Invoke-MgReplyAllUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```