---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66cde31a971038772b7085713519535ac99ec8b9
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    CountryCode = "NO"
};

await graphClient.Me.Profile.Account["{id}"]
    .Request()
    .UpdateAsync(userAccountInformation);

```