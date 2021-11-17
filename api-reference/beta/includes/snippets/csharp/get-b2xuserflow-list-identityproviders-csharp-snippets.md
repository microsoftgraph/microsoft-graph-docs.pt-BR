---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd58a2baba8cfc1405c794bb5da1e601eef653c4c6a3d2fe7b4827a4a5d899a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders
    .Request()
    .GetAsync();

```