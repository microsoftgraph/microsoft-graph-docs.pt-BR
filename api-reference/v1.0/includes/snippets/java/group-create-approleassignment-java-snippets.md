---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d520c0f3366779dae69f27c3f00746c64c99803
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780295"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = new AppRoleAssignment();
appRoleAssignment.principalId = UUID.fromString("8fce32da-1246-437b-99cd-76d1d4677bd5");
appRoleAssignment.resourceId = UUID.fromString("9028d19c-26a9-4809-8e3f-20ff73e2d75e");
appRoleAssignment.appRoleId = UUID.fromString("ef7437e6-4f94-4a0a-a110-a439eb2aa8f7");

graphClient.servicePrincipals("9028d19c-26a9-4809-8e3f-20ff73e2d75e").appRoleAssignments()
    .buildRequest()
    .post(appRoleAssignment);

```