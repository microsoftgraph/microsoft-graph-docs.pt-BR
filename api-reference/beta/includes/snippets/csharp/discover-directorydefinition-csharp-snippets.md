---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abfd04a9131987174a6a32f61d34fc35903fc3d2
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"].Schema.Directories["{directoryId}"]
    .Discover()
    .Request()
    .PostAsync();

```