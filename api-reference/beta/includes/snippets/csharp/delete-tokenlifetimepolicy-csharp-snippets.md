---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7efa60a02d7da9db7f2821155606f09bdafa7646
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42593434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.TokenLifetimePolicies["{id}"]
    .Request()
    .DeleteAsync();

```