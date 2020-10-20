---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e00a52aaa8d68b3bd1b75249788de1eedfb86a9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControls = await graphClient.ProgramControls
    .Request()
    .GetAsync();

```