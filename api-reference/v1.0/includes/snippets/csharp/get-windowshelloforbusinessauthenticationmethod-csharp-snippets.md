---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97854a0a62182f2c6f60aad269c8723beccd0255
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsHelloForBusinessAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.WindowsHelloForBusinessMethods["{windowsHelloForBusinessAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```