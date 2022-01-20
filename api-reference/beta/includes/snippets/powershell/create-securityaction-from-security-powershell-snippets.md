---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 434caeacc5284320f935775e9146d6450d3386c3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111861"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Name = "BlockIp"
    ActionReason = "Test"
    Parameters = @(
        @{
            Name = "IP"
            Value = "1.2.3.4"
        }
    )
    VendorInformation = @{
        Provider = "Windows Defender ATP"
        Vendor = "Microsoft"
    }
}

New-MgSecurityAction -BodyParameter $params

```