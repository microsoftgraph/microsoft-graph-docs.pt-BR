---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fdf7267983b422bb3000cc29628f4116a603d6dc
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536778"
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