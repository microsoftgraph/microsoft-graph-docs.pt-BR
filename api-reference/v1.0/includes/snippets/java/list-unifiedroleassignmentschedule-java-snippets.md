---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1aa44d25f0594e4313cf12cca30bc0b186cc14ae
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207181"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleCollectionPage roleAssignmentSchedules = graphClient.roleManagement().directory().roleAssignmentSchedules()
    .buildRequest()
    .get();

```