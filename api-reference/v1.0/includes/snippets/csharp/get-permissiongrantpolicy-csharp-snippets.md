---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49b916451381b60e9550b6a7d65acd3938c4837057f47b415dc2553438b70d92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272173"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"]
    .Request()
    .GetAsync();

```