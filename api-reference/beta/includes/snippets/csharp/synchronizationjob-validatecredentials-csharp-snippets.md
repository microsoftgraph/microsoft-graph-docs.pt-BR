---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a127300a62f908ab73226610dfd695e330617cbd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724970"
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