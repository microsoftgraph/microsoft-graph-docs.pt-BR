---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a9dffc6abcd60a6b406b48fd8bf673588e5eab1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099454"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "smile"
    ContentBytes = "a0b1c76de9f7="
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```