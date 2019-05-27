---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39548837e8e033276140337c3ff72d35febf2db7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"]
    .Request()
    .DeleteAsync();

```