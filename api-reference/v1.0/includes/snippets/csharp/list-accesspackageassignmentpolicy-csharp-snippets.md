---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c2ac00657509598ecf315ec18e5a3cc691e6252
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignmentPolicies = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentPolicies
    .Request()
    .GetAsync();

```