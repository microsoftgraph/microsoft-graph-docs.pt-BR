---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42a576ce62d79952db6ed54fcdee80334a9a2ec7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Filter("MentionsPreview/IsMentioned eq true,")
    .Select( e => new {
             e.Subject,
             e.Sender,
             e.ReceivedDateTime,
             e.MentionsPreview 
             })
    .GetAsync();

```