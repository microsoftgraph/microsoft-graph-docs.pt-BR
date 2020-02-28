---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7908a8177b42de90fd8c4fcf46696722ee1ba7bd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentPolicy = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentPolicies["{id}"]
    .Request()
    .GetAsync();

```