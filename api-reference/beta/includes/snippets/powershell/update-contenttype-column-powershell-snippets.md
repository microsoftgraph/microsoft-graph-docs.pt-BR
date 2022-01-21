---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c43420e1761d9c793a1d8c647ef9e5f0b0455e01
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131421"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Required = $true
    Hidden = $false
    PropagateChanges = $false
}

Update-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId -ColumnDefinitionId $columnDefinitionId -BodyParameter $params

```