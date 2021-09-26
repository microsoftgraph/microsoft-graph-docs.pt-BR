---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29e754e0fed508131a636d208b63a4c769d006d66f123029137d5c28ce3a4438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{cloudPcDeviceImage-id}"]
    .Reupload()
    .Request()
    .PostAsync();

```