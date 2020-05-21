---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98db67381715d8609ffd6637750f50a8982ff633
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336418"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.ServicePrincipals["{id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```