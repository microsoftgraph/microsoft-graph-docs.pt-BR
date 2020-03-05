---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2a4fcc4ea442d7a46a3fd55100af577b42b9b31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{id}"]
    .Request()
    .DeleteAsync();

```