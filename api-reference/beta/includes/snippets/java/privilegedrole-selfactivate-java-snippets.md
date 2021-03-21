---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4a6199468fd27a07652219080b26b041fad5dc1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974183"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "reason-value";

String duration = "duration-value";

String ticketNumber = "ticketNumber-value";

String ticketSystem = "ticketSystem-value";

graphClient.privilegedRoles("{id}")
    .selfActivate(PrivilegedRoleSelfActivateParameterSet
        .newBuilder()
        .withReason(reason)
        .withDuration(duration)
        .withTicketNumber(ticketNumber)
        .withTicketSystem(ticketSystem)
        .build())
    .buildRequest()
    .post();

```