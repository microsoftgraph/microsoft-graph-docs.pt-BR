---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a312f79942e86f8cdd57a0d08b5313c93803b034
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459007"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .Request()
    .DeleteAsync();

```