---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2be1c3f0f3a1cc606e7387c73006cb5478f2ed65ca77867e915be542e93f899c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
defaultUserRolePermissions.allowedToCreateApps = false;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```