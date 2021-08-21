---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b81d0a0aa5bbc09722f7740d5826b3e2fada4ad4c6501a21dd90f9cbc9c9ecc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213728"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = graphClient.roleManagement().directory().roleEligibilityScheduleRequests("{unifiedRoleEligibilityScheduleRequestsId}")
    .buildRequest()
    .get();

```