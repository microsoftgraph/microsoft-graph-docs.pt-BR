---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edde0e3f17002edc750be89ad4d2271bd84b3182
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].AllowedUsers["{id}"].Reference
    .Request()
    .DeleteAsync();

```