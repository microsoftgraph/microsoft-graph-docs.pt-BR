---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45820318c6c8ac8d7d41cdeae3c2bda1bdb930be
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = new EmailAuthenticationMethod
{
    EmailAddress = "kim@contoso.com"
};

await graphClient.Users["kim@contoso.com"].Authentication.EmailMethods
    .Request()
    .AddAsync(emailAuthenticationMethod);

```