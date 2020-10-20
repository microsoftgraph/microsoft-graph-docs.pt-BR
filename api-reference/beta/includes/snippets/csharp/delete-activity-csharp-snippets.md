---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a4b8f0697c1000ceafef237c88289a8ea0e4a35
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["13881113971988980728"]
    .Request()
    .DeleteAsync();

```