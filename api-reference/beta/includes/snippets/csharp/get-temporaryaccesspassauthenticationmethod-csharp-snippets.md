---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f12ef165d5e39465d1bde9ccfc742b01679de34a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = await graphClient.Users["kim@contoso.com"].Authentication.TemporaryAccessPassMethods["30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30"]
    .Request()
    .GetAsync();

```