---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78ac947d08fabd1e952580318a7d184b0a112df6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlow = new IdentityUserFlow
{
    UserFlowType = UserFlowType.SignUpOrSignIn,
    UserFlowTypeVersion = 1f
};

await graphClient.Identity.UserFlows
    .Request()
    .AddAsync(identityUserFlow);

```