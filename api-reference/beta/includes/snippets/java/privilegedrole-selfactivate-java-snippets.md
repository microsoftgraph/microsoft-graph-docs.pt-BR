---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7d306e3e20440198eef5cf978bfc300935120a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875794"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String duration = "duration-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoles("{id}")
    .selfActivate(reason,duration,ticketNumber,ticketSystem)
    .buildRequest()
    .post();

```