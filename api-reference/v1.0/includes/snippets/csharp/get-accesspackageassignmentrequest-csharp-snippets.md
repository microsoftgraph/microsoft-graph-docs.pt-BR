---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9de058a1af1563f1e97613b6347f09cd1a5ec880
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61340088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests["{accessPackageAssignmentRequest-id}"]
    .Request()
    .GetAsync();

```