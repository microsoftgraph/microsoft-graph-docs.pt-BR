---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 370a5cf7db2168b5d4140e89e0f208adda09d9421715dbf0f70e632b9b6fea0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.PasswordlessMicrosoftAuthenticatorMethods["{passwordlessMicrosoftAuthenticatorAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```