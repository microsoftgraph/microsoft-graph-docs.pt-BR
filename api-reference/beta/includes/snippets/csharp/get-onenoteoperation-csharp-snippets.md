---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbd840887e5837380483ad0e40797fb2e6331a3b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteOperation = await graphClient.Me.Onenote.Operations["{id}"]
    .Request()
    .GetAsync();

```