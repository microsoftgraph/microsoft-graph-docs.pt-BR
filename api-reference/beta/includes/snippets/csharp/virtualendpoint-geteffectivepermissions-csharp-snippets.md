---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 836e05d3ff81a8f781bde5923b48a30a34535a9794ef458345fac103fd8399af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159892"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEffectivePermissions = await graphClient.DeviceManagement.VirtualEndpoint
    .GetEffectivePermissions()
    .Request()
    .GetAsync();

```