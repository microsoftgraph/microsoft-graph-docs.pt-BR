---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5e379e410a3166b09ed85d24dd02a335332cf7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```