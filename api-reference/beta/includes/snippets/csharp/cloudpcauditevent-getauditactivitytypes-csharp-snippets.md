---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 673a272f923528117aa1f125ee3ff4be4c490ab6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAuditActivityTypes = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents
    .GetAuditActivityTypes()
    .Request()
    .GetAsync();

```