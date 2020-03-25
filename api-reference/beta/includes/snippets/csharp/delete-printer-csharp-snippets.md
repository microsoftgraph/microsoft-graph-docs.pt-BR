---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dab96c9aee02490cbfd53e6ee781c6b069459472
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948028"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"]
    .Request()
    .DeleteAsync();

```