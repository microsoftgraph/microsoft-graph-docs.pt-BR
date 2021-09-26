---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3606ea4bb1a0f424b8be3fd4af710a90af449e731bd332324fc8359731e2fac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .Request()
    .DeleteAsync();

```