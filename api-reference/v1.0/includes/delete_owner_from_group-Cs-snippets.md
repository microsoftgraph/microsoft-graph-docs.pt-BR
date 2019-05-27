---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7f565740d402c3fb59476496c958e6b2bca20bd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Owners["{id}"]
    .Request()
    .DeleteAsync();

```