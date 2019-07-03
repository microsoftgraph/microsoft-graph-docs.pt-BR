---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b27a9f0711759f53e42f7501a4f95c32128fb4eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .DismissReminder()
    .Request()
    .PostAsync();

```