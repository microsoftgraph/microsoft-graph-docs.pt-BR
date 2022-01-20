---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1cb82569c363c21a5ffa6ffeabe9d57f760a5efd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121831"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Roles = @(
        "read"
    )
}

Update-MgSitePermission -SiteId $siteId -PermissionId $permissionId -BodyParameter $params

```