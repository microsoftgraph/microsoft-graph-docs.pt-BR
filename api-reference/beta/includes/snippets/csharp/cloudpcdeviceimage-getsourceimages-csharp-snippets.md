---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c664d836ad5b0ba07ab3c4b3b21996b9de5d0a1
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSourceImages = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages
    .GetSourceImages()
    .Request()
    .GetAsync();

```