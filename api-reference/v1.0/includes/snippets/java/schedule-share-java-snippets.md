---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57f3bc559b52c989199eaa34141710643f396c557d95a3ced66f16908f1cfd31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156356"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean notifyTeam = true;

OffsetDateTime startDateTime = OffsetDateTimeSerializer.deserialize("10/08/2018 00:00:00");

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("10/15/2018 00:00:00");

graphClient.teams("{teamId}").schedule()
    .share(ScheduleShareParameterSet
        .newBuilder()
        .withNotifyTeam(notifyTeam)
        .withStartDateTime(startDateTime)
        .withEndDateTime(endDateTime)
        .build())
    .buildRequest()
    .post();

```