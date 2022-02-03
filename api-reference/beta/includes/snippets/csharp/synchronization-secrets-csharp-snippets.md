---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5aa333fe0bb148c1e711b07bf932d7d97c5a9e82
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secrets = new SynchronizationSecretKeyStringValuePair
{
    Value = new List<String>()
    {
        "",
        "",
        "",
        ""
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization
    .Request()
    .PutAsync(secrets);

```