---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b726aca7b2a62c0c051f3f39c5ae233c1ff3f7c4a36dfc87df8efe9b9a019f86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898094"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers["{scopedRoleMembership-id}"]
    .Request()
    .GetAsync();

```