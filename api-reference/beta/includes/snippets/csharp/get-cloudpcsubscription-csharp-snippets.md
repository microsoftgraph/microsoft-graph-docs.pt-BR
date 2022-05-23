---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f08fc624dee66f6c8137dc7d6974c4348057277
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSubscriptions = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots
    .GetSubscriptions()
    .Request()
    .GetAsync();

```