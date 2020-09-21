---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9329fe35cd7c4d3e39edadf6e20f382f9fbde12
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTask = new PrintTask
{
    Status = new PrintTaskStatus
    {
        State = PrintTaskProcessingState.Completed,
        Description = "completed"
    }
};

await graphClient.Print.TaskDefinitions["3203656e-6069-4e10-8147-d25290b00a3c"].Tasks["d036638b-1272-4bba-9227-732463823ed3"]
    .Request()
    .UpdateAsync(printTask);

```