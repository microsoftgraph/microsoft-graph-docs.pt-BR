---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea69878e523a8487ffe5bfefb35f4a7be3ba0e94
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118982"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#microsoft.graph.referenceAttachment"
    Name = "Personal pictures"
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
    ProviderType = "oneDriveConsumer"
    Permission = "Edit"
    IsFolder = "True"
}

New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```