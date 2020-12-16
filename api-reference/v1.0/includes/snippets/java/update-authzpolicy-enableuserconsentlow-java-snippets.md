---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9af4980a422a1d45310dc28e4c870e57d6372b18
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691363"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
DefaultUserRolePermissions defaultUserRolePermissions = new DefaultUserRolePermissions();
LinkedList<String> permissionGrantPoliciesAssignedList = new LinkedList<String>();
permissionGrantPoliciesAssignedList.add("managePermissionGrantsForSelf.microsoft-user-default-low");
defaultUserRolePermissions.permissionGrantPoliciesAssigned = permissionGrantPoliciesAssignedList;
authorizationPolicy.defaultUserRolePermissions = defaultUserRolePermissions;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```