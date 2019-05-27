---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0edb733a5f4084042f85fca2f0307955033d3f18
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472314"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataPolicyOperation = await graphClient.DataPolicyOperations["{id}"]
    .Request()
    .GetAsync();

```