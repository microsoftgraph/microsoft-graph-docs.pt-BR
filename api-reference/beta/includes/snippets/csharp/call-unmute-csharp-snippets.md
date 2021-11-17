---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 885623e01f5013343e81dbc2f813144d102a396a5e1cc28ad53578a9de7b3e41
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```