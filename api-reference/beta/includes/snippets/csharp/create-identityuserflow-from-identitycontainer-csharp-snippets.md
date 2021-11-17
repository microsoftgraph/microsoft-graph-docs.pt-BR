---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97dfa68dddee37020894139cf7a35b322f7242b30641b854cb6ed5fab7df6ebd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101998"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = new IdentityUserFlow
{
    Id = "Pol1",
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f
};

await graphClient.Identity.UserFlows
    .Request()
    .AddAsync(identityUserFlow);

```