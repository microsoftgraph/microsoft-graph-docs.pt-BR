---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18cd1c006ee324e143f35f2daf1d0681248ee1c4
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{id}"]
    .Request()
    .GetAsync();

```