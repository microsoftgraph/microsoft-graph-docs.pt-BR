---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 745fb5db33464d41117664b7dd30123d49c6c5d2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["{bucket-id}"]
    .Request()
    .GetAsync();

```