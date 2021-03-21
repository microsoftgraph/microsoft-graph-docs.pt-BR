---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9bfa2b86fd2bddb9bbe306fbfa6f16674eae4c52
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980898"
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