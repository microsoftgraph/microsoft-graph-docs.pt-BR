---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2647bb5289e3c7430fb5a685ef39188eb3792b17
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var snapshots = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots
    .Request()
    .GetAsync();

```