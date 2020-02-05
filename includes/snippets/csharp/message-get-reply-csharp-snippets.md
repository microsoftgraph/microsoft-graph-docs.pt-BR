---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c21828c7115e99308f7acb4aed7510c3eb058dbc
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADI4oeRpAABf0HJUAAA="]
    .Request()
    .GetAsync();

```