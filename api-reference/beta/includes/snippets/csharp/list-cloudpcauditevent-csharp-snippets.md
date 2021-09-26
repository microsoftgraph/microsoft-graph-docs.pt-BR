---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e5918054e0c65dec7762de0cb1902b7b6692ede48cb1caefc41d14bbf746680
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditEvents = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents
    .Request()
    .GetAsync();

```