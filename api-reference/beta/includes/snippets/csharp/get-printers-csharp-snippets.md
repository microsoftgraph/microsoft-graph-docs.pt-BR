---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1efb91f1ccc180417c1912315a178695bbb0446
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printers = await graphClient.Print.Printers
    .Request()
    .GetAsync();

```