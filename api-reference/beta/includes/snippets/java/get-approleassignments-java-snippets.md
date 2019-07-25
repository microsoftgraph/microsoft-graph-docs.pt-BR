---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a496b70ecc5792b8fe2688467ab4ea50938640c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870090"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.servicePrincipals("{id}").appRoleAssignments()
    .buildRequest()
    .get();

```