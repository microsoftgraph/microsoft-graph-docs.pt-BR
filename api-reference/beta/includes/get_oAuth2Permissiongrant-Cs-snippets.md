---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 862461123e27ff29166814b0d342497e5573f07d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .GetAsync();

```