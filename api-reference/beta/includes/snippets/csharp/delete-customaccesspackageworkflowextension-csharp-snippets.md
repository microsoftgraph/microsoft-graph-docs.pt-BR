---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae86c21e76b07a6a84c37fc5b6311e665f7dcfe2
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"].CustomAccessPackageWorkflowExtensions["{customAccessPackageWorkflowExtension-id}"]
    .Request()
    .DeleteAsync();

```