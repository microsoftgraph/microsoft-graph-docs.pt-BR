---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b12f0750cfbdaf7e200f60fddc2419dfc6dc698e22c94bdb20c0059cbdb7984c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100183"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var phoneAuthenticationMethod = new PhoneAuthenticationMethod
{
    PhoneNumber = "+1 2065555555",
    PhoneType = AuthenticationPhoneType.Mobile
};

await graphClient.Me.Authentication.PhoneMethods
    .Request()
    .AddAsync(phoneAuthenticationMethod);

```