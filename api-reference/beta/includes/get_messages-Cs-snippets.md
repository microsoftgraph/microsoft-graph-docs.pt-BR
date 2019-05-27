---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca5b571dad3993a594da8b1197e4437174a38d76
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Me.Messages
    .Request()
    .Select( e => new {
             e.Sender,
             e.Subject 
             })
    .GetAsync();

```