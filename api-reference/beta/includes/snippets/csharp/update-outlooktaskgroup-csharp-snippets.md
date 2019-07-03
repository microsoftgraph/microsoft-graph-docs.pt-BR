---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27310935ac5bee281f55e1d70e572e5e911895cd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477504"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskGroup = new OutlookTaskGroup
{
    Name = "Personal Tasks"
};

await graphClient.Me.Outlook.TaskGroups["AAMkADIyAAAhrbe-AAA="]
    .Request()
    .UpdateAsync(outlookTaskGroup);

```