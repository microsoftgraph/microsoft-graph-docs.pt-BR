---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1f7a2578d2e4c4405f041eb0a0fdc37447baf82
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = await graphClient.Policies.AccessReviewPolicy
    .Request()
    .GetAsync();

```