---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59a7bf4f81e2483a5a8318da07bbf667ceed3303
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UnifiedRoleAssignmentCollectionPage transitiveRoleAssignments = graphClient.roleManagement().directory().transitiveRoleAssignments()
    .buildRequest( requestOptions )
    .filter("principalId eq '2c7936bc-3517-40f3-8eda-4806637b6516' and directoryScopeId eq '/administrativeUnits/26e79164-0c5c-4281-8c5b-be7bc7809fb2'")
    .get();

```