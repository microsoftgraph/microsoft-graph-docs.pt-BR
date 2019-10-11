---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af0d59e99448d80ebf5e6ba88610ee717d4ab9f9
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReplyAll(null,null)
    .Request()
    .PostAsync();

```