---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f59b1f04924b6d9f82b8134530714a40e6c3759
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131855"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Labels = @(
        @{
            LanguageTag = "en-US"
            Name = "Car"
            IsDefault = $true
        }
    )
}

New-MgSiteTermStoreSetChild -SiteId $siteId -SetId $setId -BodyParameter $params

```