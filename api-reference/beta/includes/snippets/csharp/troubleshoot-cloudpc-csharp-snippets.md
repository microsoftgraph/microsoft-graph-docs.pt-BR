---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29d6e09cd832f7ba9c005ac68bdb02e5c25cb1b6
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61523652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Troubleshoot()
    .Request()
    .PostAsync();

```