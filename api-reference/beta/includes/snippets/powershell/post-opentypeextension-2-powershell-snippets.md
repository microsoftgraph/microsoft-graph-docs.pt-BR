---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7ecac0bd291a818db374e4c5f33f73ddd0a2e26
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130926"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.openTypeExtension"
    ExtensionName = "Com.Contoso.Referral"
    CompanyName = "Wingtip Toys"
    DealValue = 
    ExpirationDate = "2015-12-03T10:00:00.000Z"
}

New-MgUserMessageExtension -UserId $userId -MessageId $messageId -BodyParameter $params

```