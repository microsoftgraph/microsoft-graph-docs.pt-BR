---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22c8ff73c0d788be08a98f46a6dc174c786f51fbba6fe1e815aa34ad7cde88b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String message = "Approved!";

graphClient.teams("{teamId}").schedule().offerShiftRequests("{offerShiftRequestId}")
    .approve(ScheduleChangeRequestApproveParameterSet
        .newBuilder()
        .withMessage(message)
        .build())
    .buildRequest()
    .post();

```