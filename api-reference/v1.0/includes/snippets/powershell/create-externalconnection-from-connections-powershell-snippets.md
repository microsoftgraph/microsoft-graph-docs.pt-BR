---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1761c5114edd13b3a37d0584b6990e0b2949406c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107457"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    Id = "contosohr"
    Name = "Contoso HR"
    Description = "Connection to index Contoso HR system"
}

New-MgExternalConnection -BodyParameter $params

```