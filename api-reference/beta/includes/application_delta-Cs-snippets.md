---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2216615d76ce96277f66e05536975f5a227f9d5a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Applications.Delta()
    .Request()
    .GetAsync();

```