---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db0defaf37ccb177a5000aa49d093830a819a92c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignment unifiedRoleAssignment = new UnifiedRoleAssignment();
unifiedRoleAssignment.roleDefinitionId = "fe930be7-5e62-47db-91af-98c3a49a38b1";
unifiedRoleAssignment.principalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d";
unifiedRoleAssignment.directoryScopeId = "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a";

graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignment);

```