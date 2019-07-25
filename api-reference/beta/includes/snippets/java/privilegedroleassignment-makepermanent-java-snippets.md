---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b00cb9cae5b4edc9d1f9c05060f50a4a502ff6c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875676"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoleAssignments("{id}")
    .makePermanent(reason,ticketNumber,ticketSystem)
    .buildRequest()
    .post();

```