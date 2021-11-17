---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ead67a76d627f31ad417bb0bcefb14713d818dbc3501cc77254eeadc0f042e49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationJob = new SynchronizationJob
{
    TemplateId = "BoxOutDelta"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs
    .Request()
    .AddAsync(synchronizationJob);

```