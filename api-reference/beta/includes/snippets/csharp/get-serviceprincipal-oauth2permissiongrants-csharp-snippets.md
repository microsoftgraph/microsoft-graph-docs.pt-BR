---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 587cf4d523c791febe5b50c26adfba44b047f3398e365d07645352d3d0c88e7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099617"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oauth2PermissionGrants = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Oauth2PermissionGrants
    .Request()
    .GetAsync();

```