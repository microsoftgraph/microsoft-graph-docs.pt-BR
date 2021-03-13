---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bab54ee58b6e2479cd5947ff2f0023734bd297a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAuthenticationMethod = new EmailAuthenticationMethod
{
    EmailAddress = "kim@contoso.com"
};

await graphClient.Users["{user-id}"].Authentication.EmailMethods
    .Request()
    .AddAsync(emailAuthenticationMethod);

```