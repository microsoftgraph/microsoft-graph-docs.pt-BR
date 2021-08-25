---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 526d76f6cd1ea60e4625b576e55d7418e1d929ef
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516012"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilitySchedule unifiedRoleEligibilitySchedule = graphClient.roleManagement().directory().roleEligibilitySchedules("313af44a-07c9-43a7-9970-5072a6b5591f")
    .buildRequest()
    .get();

```