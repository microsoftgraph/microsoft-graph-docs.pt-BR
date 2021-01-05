---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4017ee7f5444106aecd87cd802d50ac5cc664b12
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parameters = new List<SynchronizationJobApplicationParameters>()
{
    new SynchronizationJobApplicationParameters
    {
        Subjects = new List<SynchronizationJobSubject>()
        {
            new SynchronizationJobSubject
            {
                ObjectId = "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
                ObjectTypeName = "User"
            }
        },
        RuleId = "ea807875-5618-4f0a-9125-0b46a05298ca"
    }
};

await graphClient.ServicePrincipals["{servicePrincipalsId}"].Synchronization.Jobs["{synchronizationJobId}"]
    .ProvisionOnDemand(parameters)
    .Request()
    .PostAsync();

```