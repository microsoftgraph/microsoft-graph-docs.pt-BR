---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e77f3db11d06214bfbe723ccb9d67151737fe3f5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350535"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "smile"
    ContentBytes = "R0lGODdhEAYEAA7"
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```