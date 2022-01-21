---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ced167eb03d7982ae72d6da5652b423f822a8746
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097081"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    EmailAddresses = @(
        @{
            Type = "personal"
            Name = "Pavel Bansky"
            Address = "pavelb@adatum.onmicrosoft.com"
        }
        @{
            Address = "pavelb@fabrikam.onmicrosoft.com"
            Name = "Pavel Bansky"
            Type = "other"
            OtherLabel = "Volunteer work"
        }
    )
}

Update-MgUserContact -UserId $userId -ContactId $contactId -BodyParameter $params

```