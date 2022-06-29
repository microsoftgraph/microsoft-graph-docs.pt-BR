---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2dca18224c2c14367289a5502fd0aef3b6987ee
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = new TemporaryAccessPassAuthenticationMethod
{
    StartDateTime = DateTimeOffset.Parse("2022-06-05T00:00:00Z"),
    LifetimeInMinutes = 60,
    IsUsableOnce = false
};

await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods
    .Request()
    .AddAsync(temporaryAccessPassAuthenticationMethod);

```