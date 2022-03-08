---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 760bd500730556f59240caa38e5a1e5ad3dd8930
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333040"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{accessPackageAssignmentPolicy-id}"]
    .Request()
    .Expand("customExtensionHandlers($expand=customExtension)")
    .GetAsync();

```