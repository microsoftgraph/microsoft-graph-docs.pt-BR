---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0a3bf46d1b0b44cf41c35eefd6eb02ade4cf71f890dc2d93914a027bced33d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentResourceRole = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentResourceRoles["{accessPackageAssignmentResourceRole-id}"]
    .Request()
    .GetAsync();

```