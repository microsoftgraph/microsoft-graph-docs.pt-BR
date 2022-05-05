---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a146cc15ba5245a2a21c2481ca0fd5ed614aeff
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstanceCollectionPage roleAssignmentScheduleInstances = graphClient.roleManagement().directory().roleAssignmentScheduleInstances()
    .buildRequest()
    .get();

```