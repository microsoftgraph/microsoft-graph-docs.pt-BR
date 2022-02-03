---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ecb3c9468b0691d2d5293d19f596680bc9cda18
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341213"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPC = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Request()
    .GetAsync();

```