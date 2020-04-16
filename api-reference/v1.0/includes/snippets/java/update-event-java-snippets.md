---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cb09248228596c81736feed44f61b01d5267cc6
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43512284"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.originalStartTimeZone = "originalStartTimeZone-value";
event.originalEndTimeZone = "originalEndTimeZone-value";
ResponseStatus responseStatus = new ResponseStatus();
responseStatus.response = ResponseType.NONE;
responseStatus.time = "datetime-value";
event.responseStatus = responseStatus;
event.recurrence = null;
event.iCalUId = "iCalUId-value";
event.reminderMinutesBeforeStart = 99;
event.isOnlineMeeting = true;
event.onlineMeetingProvider = "teamsForBusiness";
event.isReminderOn = true;

graphClient.me().events("{id}")
    .buildRequest()
    .patch(event);

```