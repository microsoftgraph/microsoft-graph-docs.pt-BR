---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3afef900027a1a3bf9e7a4b4f1a226887c993379df2ddb66baf382397894b2ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new SynchronizationJobRestartCriteria
{
    ResetScope = SynchronizationJobRestartScope.Escrows | SynchronizationJobRestartScope.Watermark | SynchronizationJobRestartScope.QuarantineState
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Restart(criteria)
    .Request()
    .Header("Authorization","Bearer <token>")
    .PostAsync();

```