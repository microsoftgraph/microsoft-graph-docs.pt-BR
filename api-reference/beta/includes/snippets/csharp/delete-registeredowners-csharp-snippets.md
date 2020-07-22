---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f18be5eb63dac0099dc670492d75e5af24a77b6
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{id}"].RegisteredOwners["{id}"].Reference
    .Request()
    .DeleteAsync();

```