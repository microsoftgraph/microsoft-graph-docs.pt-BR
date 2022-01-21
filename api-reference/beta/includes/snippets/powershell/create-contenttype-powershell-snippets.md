---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 643a2f8593d77a2a7d8d64c3858db6a39ec42513
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125220"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Name = "docSet"
    Description = "custom docset"
    Base = @{
        Name = "Document Set"
        Id = "0x0120D520"
    }
    Group = "Document Set Content Types"
}

New-MgSiteContentType -SiteId $siteId -BodyParameter $params

```