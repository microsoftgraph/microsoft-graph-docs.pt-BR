---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb152f6b2684b88f3ef1052c78fc27e8efe94f31
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDeviceImage = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{cloudPcDeviceImage-id}"]
    .Request()
    .GetAsync();

```