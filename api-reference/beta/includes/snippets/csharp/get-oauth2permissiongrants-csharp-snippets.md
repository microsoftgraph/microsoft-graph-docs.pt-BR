---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98db67381715d8609ffd6637750f50a8982ff633
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.ServicePrincipals["{id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```