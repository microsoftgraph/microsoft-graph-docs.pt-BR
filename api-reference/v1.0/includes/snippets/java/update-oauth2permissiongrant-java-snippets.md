---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9aba4dfc821868f3e887e596ff0e2166eca753ec
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335257"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.scope = "scope-value";

graphClient.oauth2PermissionGrants("{id}")
    .buildRequest()
    .patch(oAuth2PermissionGrant);

```