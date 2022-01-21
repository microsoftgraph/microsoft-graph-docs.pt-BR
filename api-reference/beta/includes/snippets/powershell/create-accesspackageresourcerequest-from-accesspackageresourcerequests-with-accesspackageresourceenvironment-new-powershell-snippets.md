---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3fe151112b02a0c69e70c00cbb948c874c4846f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119053"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    CatalogId = "de9315c1-272b-4905-924b-cc112ca180c7"
    AccessPackageResource = @{
        DisplayName = "Community Outreach"
        Description = "https://contoso.sharepoint.com/sites/CSR"
        ResourceType = "SharePoint Online Site"
        OriginId = "https://contoso.sharepoint.com/sites/CSR"
        OriginSystem = "SharePointOnline"
        AccessPackageResourceEnvironment = @{
            OriginId = "https://contoso-admin.sharepoint.com/"
        }
    }
    RequestType = "AdminAdd"
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```