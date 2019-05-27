---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d898d15e5529c6dd93e293b79ffc7273a8e90343
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Settings["{id}"]
    .Request()
    .DeleteAsync();

```