---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be8363a1bcaa31f6669164b082f1ca77217e93f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976455"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
defaultUserRolePermissions.allowedToCreateApps = false;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```