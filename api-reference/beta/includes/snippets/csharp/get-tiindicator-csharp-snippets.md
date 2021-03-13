---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5642d818c13d9bd0a432176ab21a71dd483d7c35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797260"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .GetAsync();

```