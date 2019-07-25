---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26a7a56142188af60d369178ed864cb7ba4a3bad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["3162F1E1-C4C0-604B-51D8-91DA78989EB1"]
    .Request()
    .GetAsync();

```