---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c01f678c77faa3931dd197b59458474b8b4a994
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343167"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Subject = "Meet for lunch?"
        Body = @{
            ContentType = "Text"
            Content = "The new cafeteria is open."
        }
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "fannyd@contoso.onmicrosoft.com"
                }
            }
        )
        CcRecipients = @(
            @{
                EmailAddress = @{
                    Address = "danas@contoso.onmicrosoft.com"
                }
            }
        )
    }
    SaveToSentItems = "false"
}

# A UPN can also be used as -UserId.
Send-MgUserMail -UserId $userId -BodyParameter $params

```