---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27d65cfce4160823eade681ced55926c68a9fb15
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041937"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGI1AAAoZCfHAAA="]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select( e => new {
             e.Subject,
             e.Body,
             e.BodyPreview,
             e.UniqueBody 
             })
    .GetAsync();

```