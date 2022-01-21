---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0ea9d2a0d3175526b2ac90caf121fe5f1a7aa72
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111686"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Name = "Events.aspx"
    Title = "Team Events"
    PublishingState = @{
        Level = "checkedOut"
        VersionId = "0.1"
    }
    WebParts = @(
        @{
            Type = "rte"
            Data = @{
                InnerHTML = "<p>Here are the team's upcoming events:</p>"
            }
        }
        @{
            Type = "d1d91016-032f-456d-98a4-721247c305e8"
            Data = @{
                Title = "Events"
                Description = "Display upcoming events"
                DataVersion = "1.0"
            }
        }
    )
}

New-MgSitePage -SiteId $siteId -BodyParameter $params

```