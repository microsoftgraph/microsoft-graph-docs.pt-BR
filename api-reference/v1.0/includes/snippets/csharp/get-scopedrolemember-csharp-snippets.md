---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc94ba21b35458db105494176159f8070c81f6e1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49984943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = await graphClient.Directory.AdministrativeUnits["{id}"].ScopedRoleMembers["{id}"]
    .Request()
    .GetAsync();

```