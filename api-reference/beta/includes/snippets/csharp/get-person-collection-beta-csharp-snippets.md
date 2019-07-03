---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7ec8819005c21715473378fe105484d3c0f26e6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var people = await graphClient.Me.People
    .Request()
    .GetAsync();

```