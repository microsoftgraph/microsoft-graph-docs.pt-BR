---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d395f1ee7ba83dbef4ff79dc7855654ee4dd5257
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130923"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "Annual review"
    Body = @{
        ContentType = "HTML"
        Content = "You should be proud!"
    }
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "rufus@contoso.com"
            }
        }
    )
    Extensions = @(
        @{
            "@odata.type" = "microsoft.graph.openTypeExtension"
            ExtensionName = "Com.Contoso.Referral"
            CompanyName = "Wingtip Toys"
            ExpirationDate = "2015-12-30T11:00:00.000Z"
            DealValue = 
        }
    )
}

New-MgUserMessage -UserId $userId -BodyParameter $params

```