---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 505d4e87a55251d204451a35f4bb73d69670e0f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131288"
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

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```