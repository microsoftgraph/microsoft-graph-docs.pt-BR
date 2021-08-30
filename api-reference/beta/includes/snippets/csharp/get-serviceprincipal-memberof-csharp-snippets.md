---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3d21cab38e9aa756f790661e9f43613bd9f4413574e7fe3995afe262c324695
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.ServicePrincipals["{servicePrincipal-id}"].MemberOf
    .Request()
    .GetAsync();

```