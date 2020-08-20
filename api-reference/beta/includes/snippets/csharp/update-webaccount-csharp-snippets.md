---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8f8ff9d985a22bee3bc5ec4f41b3c788a3c8336
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = new WebAccount
{
    WebUrl = "https://github.com/innocenty.popov"
};

await graphClient.Me.Profile.WebAccounts["{id}"]
    .Request()
    .UpdateAsync(webAccount);

```