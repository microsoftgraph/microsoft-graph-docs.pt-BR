---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 787ad4adaef88925158e2aa4df9cb3ac58628821a5fe3fceadad3f337d6425bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159645"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTask = new OutlookTask
{
    DueDateTime = new DateTimeTimeZone
    {
        DateTime = "2016-05-06T16:00:00",
        TimeZone = "Eastern Standard Time"
    }
};

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .Header("Prefer","outlook.timezone=\"Eastern Standard Time\"")
    .UpdateAsync(outlookTask);

```