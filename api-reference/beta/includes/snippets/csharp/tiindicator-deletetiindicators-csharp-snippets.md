---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 691b4ae1633ce91fa60e274e9743edd52ef72755
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611577"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "id-value1",
    "id-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicators(value)
    .Request()
    .PostAsync();

```