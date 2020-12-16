---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebd39236355a18eefcd78c8df09e2dc9be5b2464
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    AllowEmailVerifiedUsersToJoinOrganization = false
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```