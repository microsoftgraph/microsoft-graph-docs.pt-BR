---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08e51183e1d030780318741ad7b5323dc6c121607b67e24780d65c5fdf22e794
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicies = await graphClient.Policies.PermissionGrantPolicies
    .Request()
    .GetAsync();

```