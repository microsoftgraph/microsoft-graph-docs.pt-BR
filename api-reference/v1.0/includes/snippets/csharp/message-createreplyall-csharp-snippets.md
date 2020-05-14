---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af0d59e99448d80ebf5e6ba88610ee717d4ab9f9
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "37428759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReplyAll(null,null)
    .Request()
    .PostAsync();

```