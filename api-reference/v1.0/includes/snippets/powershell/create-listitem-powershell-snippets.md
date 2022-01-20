---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b9fc3ec10abff026af42a86b5ed89b9ba39e7ff
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128704"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Fields = @{
        Title = "Widget"
        Color = "Purple"
        Weight = 
    }
}

New-MgSiteListItem -SiteId $siteId -ListId $listId -BodyParameter $params

```