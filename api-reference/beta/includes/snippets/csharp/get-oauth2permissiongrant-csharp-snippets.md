---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 862461123e27ff29166814b0d342497e5573f07d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476165"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .GetAsync();

```