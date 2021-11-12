---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 665854157bf14a694f869ed2e3a0849ea1800735552d18ec1ae81d58e3d58bea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["{event-id}"]
    .Request()
    .Select("subject,body,bodyPreview,organizer,attendees,start,end,location,locations")
    .GetAsync();

```