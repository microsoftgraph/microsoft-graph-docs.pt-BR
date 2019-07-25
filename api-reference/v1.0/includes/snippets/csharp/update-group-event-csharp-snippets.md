---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdf7267983b422bb3000cc29628f4116a603d6dc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722596"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = new Event
{
    Location = new Location
    {
        DisplayName = "Conf Room 2"
    }
};

await graphClient.Groups["01d4ee64-15ce-491e-bad1-b91aa3223df4"].Calendar.Events["AAMkADZlAAAAABERAAA="]
    .Request()
    .UpdateAsync(@event);

```