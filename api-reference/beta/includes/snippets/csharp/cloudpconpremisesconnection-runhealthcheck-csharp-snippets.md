---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 569eb3646b271f9b584c308dd44fa569fbc33597
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{id}"]
    .Reprovision()
    .Request()
    .PostAsync();

```