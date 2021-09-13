---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71073eb4716e644634bb269e32128b192d9ad4a31a651d8abe991f3304d61f14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```