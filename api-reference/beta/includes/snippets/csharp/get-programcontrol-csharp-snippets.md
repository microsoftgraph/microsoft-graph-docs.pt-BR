---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e00a52aaa8d68b3bd1b75249788de1eedfb86a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var programControls = await graphClient.ProgramControls
    .Request()
    .GetAsync();

```