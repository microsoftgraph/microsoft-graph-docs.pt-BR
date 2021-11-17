---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e59485587e838c9ac9a383e564266b680205a6d45d4ab9cee99f2a8c49ea28e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicies = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies
    .Request()
    .GetAsync();

```