---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 587e3665e7ceedf0ce850c077d2493d4029a1e2c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344556"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    HubSiteUrls = @(
        "https://graph.microsoft.com/beta/sites/id"
    )
    PropagateToExistingLists = $false
}

Join-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```