---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ec60b91bfea6a8ace8d6a03b1d38125de95e175fd8bb4e3e3da2d8652482200
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214983"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["{event-id}"]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select("subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees")
    .GetAsync();

```