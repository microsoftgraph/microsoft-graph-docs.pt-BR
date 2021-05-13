---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a146cc15ba5245a2a21c2481ca0fd5ed614aeff
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475167"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstanceCollectionPage roleAssignmentScheduleInstances = graphClient.roleManagement().directory().roleAssignmentScheduleInstances()
    .buildRequest()
    .get();

```