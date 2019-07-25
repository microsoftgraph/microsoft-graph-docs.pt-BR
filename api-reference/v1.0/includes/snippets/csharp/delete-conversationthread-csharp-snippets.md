---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 070506d6496492be405a4e7691c0fcf4bbebb908
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .DeleteAsync();

```