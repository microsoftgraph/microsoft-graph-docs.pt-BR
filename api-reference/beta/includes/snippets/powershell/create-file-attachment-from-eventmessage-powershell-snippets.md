---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9d673625bb29425082c4c1cd02829a090d1cc77
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351661"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#Microsoft.OutlookServices.FileAttachment"
    Name = "name-value"
    ContentType = "contentType-value"
    IsInline = $false
    ContentLocation = "contentLocation-value"
    ContentBytes = "contentBytes-value"
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```