---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b61de7c8e10ae8e09d88b25d09a37bc0ab727fc3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60717975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var continuousAccessEvaluationPolicy = new ContinuousAccessEvaluationPolicy
{
    Migrate = true
};

await graphClient.Identity.ContinuousAccessEvaluationPolicy
    .Request()
    .UpdateAsync(continuousAccessEvaluationPolicy);

```