---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8989dde3e99e0de70a465e4bd76cc99728581187a0bc41db7c0df6228528d42d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
    AppRoleAssignmentRequired = true
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .UpdateAsync(servicePrincipal);

```