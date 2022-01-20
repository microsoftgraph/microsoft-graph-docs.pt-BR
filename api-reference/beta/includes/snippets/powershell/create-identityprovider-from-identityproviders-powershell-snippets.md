---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0e210664d31ed832e5f210bbcf2380bed4fe5a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090025"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "microsoft.graph.identityProvider"
    Name = "Login with Amazon"
    Type = "Amazon"
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8"
    ClientSecret = "000000000000"
}

New-MgIdentityProvider -BodyParameter $params

```