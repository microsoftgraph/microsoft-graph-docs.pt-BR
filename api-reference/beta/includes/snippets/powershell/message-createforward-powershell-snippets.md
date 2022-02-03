---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58f17adcfc92a7faeed65bdf2aad5f475b4e5384
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341641"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        IsDeliveryReceiptRequested = $true
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "danas@contoso.onmicrosoft.com"
                    Name = "Dana Swope"
                }
            }
        )
    }
    Comment = "Dana, just want to make sure you get this; you'll need this if the project gets approved."
}

# A UPN can also be used as -UserId.
New-MgUserMessageForward -UserId $userId -MessageId $messageId -BodyParameter $params

```