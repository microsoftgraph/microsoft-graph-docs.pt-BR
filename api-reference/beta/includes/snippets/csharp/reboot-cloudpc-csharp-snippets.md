---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01b9dc93728493bdc1fda9b7aba9fa8ed9b74fa6
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524428"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Reboot()
    .Request()
    .PostAsync();

```