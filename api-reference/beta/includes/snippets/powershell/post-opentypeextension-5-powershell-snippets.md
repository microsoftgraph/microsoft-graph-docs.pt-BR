---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d48a61ce791b3ad16c044b91e558460160a0f43f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130924"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Topic = "Does anyone have a second?"
    Threads = @(
        @{
            Posts = @(
                @{
                    Body = @{
                        ContentType = "HTML"
                        Content = "This is urgent!"
                    }
                    Extensions = @(
                        @{
                            "@odata.type" = "microsoft.graph.openTypeExtension"
                            ExtensionName = "Com.Contoso.Benefits"
                            CompanyName = "Contoso"
                            ExpirationDate = "2016-08-03T11:00:00.000Z"
                            TopPicks = @(
                                "Employees only"
                                "Add spouse or guest"
                                "Add family"
                            )
                        }
                    )
                }
            )
        }
    )
}

New-MgGroupConversation -GroupId $groupId -BodyParameter $params

```