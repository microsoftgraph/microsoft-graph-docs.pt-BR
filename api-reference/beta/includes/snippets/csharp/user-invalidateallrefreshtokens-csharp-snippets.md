---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59bf2b57c658d0633094613383d7524d43c8085f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .InvalidateAllRefreshTokens()
    .Request()
    .PostAsync();

```