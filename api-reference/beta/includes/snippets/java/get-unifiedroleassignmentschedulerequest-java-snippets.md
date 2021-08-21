---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ec26a150f20d819c04f8cf023b3e5782cf9fbe77940981a67222a06622a7cc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = graphClient.roleManagement().directory().roleAssignmentScheduleRequests("{unifiedRoleAssignmentScheduleRequestsId}")
    .buildRequest()
    .get();

```