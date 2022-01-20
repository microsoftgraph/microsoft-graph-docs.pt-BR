---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34ebc4d8d26c9c77173671755ddc5e231b997c7c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099545"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Color = "Fuchsia"
    Quantity = 
}

Update-MgSiteListItemField -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```