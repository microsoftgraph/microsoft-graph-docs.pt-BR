---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e64969734186bcab996b5895c2561f4e5ba7b415a438e8cce24aa86dba1924bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271966"
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