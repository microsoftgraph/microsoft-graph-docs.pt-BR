---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91e67907ae428279d4c8960de4ed6f9268be3561
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = await graphClient.Oauth2permissiongrants["delta"]
    .Request()
    .GetAsync();

```