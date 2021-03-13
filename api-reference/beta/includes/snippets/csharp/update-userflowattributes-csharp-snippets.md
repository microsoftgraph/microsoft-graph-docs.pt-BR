---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b0ba1cfb3d11b96de49ffc54334c4159105fc4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = new IdentityUserFlowAttribute
{
    Description = "Your new hobby"
};

await graphClient.Identity.UserFlowAttributes["{identityUserFlowAttribute-id}"]
    .Request()
    .UpdateAsync(identityUserFlowAttribute);

```