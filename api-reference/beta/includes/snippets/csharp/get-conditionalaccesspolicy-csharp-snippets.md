---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 513ddffef8ac7a35133ca6bab402346d0c66b02d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = await graphClient.ConditionalAccess.Policies["{id}"]
    .Request()
    .GetAsync();

```