---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303d24a6b10ce801e1c55c278ac9da906e886bc8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458542"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Onenote.Pages["{id}"]
    .Request()
    .DeleteAsync();

```