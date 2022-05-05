---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8615a6d460428fbb81bbb2bfe999e96616021d54
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205233"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleInstance unifiedRoleAssignmentScheduleInstance = graphClient.roleManagement().directory().roleAssignmentScheduleInstances("lAPpYvVpN0KRkAEhdxReEJ2SvT9WjGJEhR4OuaezoqU-1")
    .buildRequest()
    .get();

```