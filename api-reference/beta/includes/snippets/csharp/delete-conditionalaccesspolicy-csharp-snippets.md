---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4a6894052d762c94803499df0dae4e5482ce3a3
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127139"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.Policies["{id}"]
    .Request()
    .DeleteAsync();

```