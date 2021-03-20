---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5a9d11661a100af93acdbdb8dae9939bf36b80c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Reprovision()
    .Request()
    .PostAsync();

```