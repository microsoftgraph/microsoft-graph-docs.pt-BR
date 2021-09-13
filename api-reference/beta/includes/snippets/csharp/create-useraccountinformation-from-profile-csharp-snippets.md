---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16e33ce2907f1c074b01a36e4c9dad0e4fdd259e0ca97d2f58da0ff42507371a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    AllowedAudiences = AllowedAudiences.Organization,
    CountryCode = "NO"
};

await graphClient.Me.Profile.Account
    .Request()
    .AddAsync(userAccountInformation);

```