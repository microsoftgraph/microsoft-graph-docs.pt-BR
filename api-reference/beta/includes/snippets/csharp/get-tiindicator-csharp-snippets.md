---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba7f735e60d154713f5ea9655d7403992b0f5522005ca611b2af778b6de11467
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tiIndicator = await graphClient.Security.TiIndicators["{tiIndicator-id}"]
    .Request()
    .GetAsync();

```