---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0108ec1872653616bbe4afdf50d9bbc4be845e69
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565861"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskTrigger = new PrintTaskTrigger
{
    Event = PrintEvent.JobStarted,
    AdditionalData = new Dictionary<string, object>()
    {
        {"definition@odata.bind", "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"}
    }
};

await graphClient.Print.Printers["ae63f617-4856-4b45-8ea9-69dfbeea230e"].TaskTriggers
    .Request()
    .AddAsync(printTaskTrigger);

```