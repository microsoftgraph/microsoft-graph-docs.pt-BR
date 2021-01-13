---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb6c007dee1e4d3501ff0c8b51bdacb80ae05ab5
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["15d889df-3eb8-4e9b-bfb4-b1908849aec4"].AccessPackageResourceRoles
    .Request()
    .Filter("(originSystem eq 'AadGroup' and accessPackageResource/id eq 'a35bef72-a8aa-4ca3-af30-f6b2ece7208f'),")
    .Expand("accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')")
    .GetAsync();

```