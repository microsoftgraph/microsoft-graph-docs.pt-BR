---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca341ed6cf1cf43dbbf8df1f0c438a77695155e6c6761b9fbf4d86de6cd668f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignment privilegedRoleAssignment = new PrivilegedRoleAssignment();
privilegedRoleAssignment.userId = "userId-value";
privilegedRoleAssignment.roleId = "roleId-value";

graphClient.privilegedRoleAssignments()
    .buildRequest()
    .post(privilegedRoleAssignment);

```