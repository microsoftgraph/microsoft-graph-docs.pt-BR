---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66344267667a838709075994d7216f1ae60c9be644deb337682732ff43f31dc9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"]
    .Request()
    .DeleteAsync();

```