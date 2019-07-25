---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 827baec86d11ce2ee3af4671531c2c27444ab467
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkAGIAAAoZDOFAAA="]
    .Request()
    .Header("Prefer","outlook.timezone=\"Pacific Standard Time\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview,
             e.Organizer,
             e.Attendees,
             e.Start,
             e.End,
             e.Location 
             })
    .GetAsync();

```