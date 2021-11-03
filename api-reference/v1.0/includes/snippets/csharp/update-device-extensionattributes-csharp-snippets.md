---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f9b6a7815cc9e9a4369d261a43840bdd3e17530
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"extensionAttributes", "{\"extensionAttribute1\":\"BYOD-Device\"}"}
    }
};

await graphClient.Devices["{device-id}"]
    .Request()
    .UpdateAsync(device);

```