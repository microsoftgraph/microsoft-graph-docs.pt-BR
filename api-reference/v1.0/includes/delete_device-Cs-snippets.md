---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab8bde42fb4ca337230599efbf7c4da029724608
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"]
    .Request()
    .DeleteAsync();

```