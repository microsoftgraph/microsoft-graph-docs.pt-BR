---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a127300a62f908ab73226610dfd695e330617cbd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentials = new List<SynchronizationSecretKeyStringValuePair>()
{
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.UserName,
        Value = "user@domain.com"
    },
    new SynchronizationSecretKeyStringValuePair
    {
        Key = SynchronizationSecret.Password,
        Value = "password-value"
    }
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{id}"]
    .ValidateCredentials(applicationIdentifier,templateId,useSavedCredentials,credentials)
    .Request()
    .PostAsync();

```