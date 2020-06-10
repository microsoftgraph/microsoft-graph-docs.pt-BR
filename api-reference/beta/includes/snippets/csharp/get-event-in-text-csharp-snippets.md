---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e067ef5387f53a443adbe4184216149c396bf394
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Events["AAMkAGI1AAAoZDOFAAA="]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview")
    .GetAsync();

```