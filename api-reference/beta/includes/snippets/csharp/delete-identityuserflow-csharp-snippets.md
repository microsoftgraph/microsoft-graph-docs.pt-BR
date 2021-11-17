---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e84b53d2d6fbc6a483eb3feff137ce0f1df53016f5f8f0c6c0872f9a181ce302
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326737"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```