---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76b9501c0ee516e3f079ab89da4fcf640f2afed6
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.DeviceManagement.RoleAssignments["lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1"]
    .Request()
    .DeleteAsync();

```