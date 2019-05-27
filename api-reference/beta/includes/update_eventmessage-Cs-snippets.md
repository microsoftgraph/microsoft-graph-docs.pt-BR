---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa38368f00ba725d180f9c4d6e7a6b93c7570795
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    IsRead = "true"
};

await graphClient.Me.Messages["{id}"]
    .Request()
    .UpdateAsync(message);

```