---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d36d33b93c22d7482a6092deef47ac3e8e55e03
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
event.originalStartTimeZone = "originalStartTimeZone-value";
event.originalEndTimeZone = "originalEndTimeZone-value";
ResponseStatus responseStatus = new ResponseStatus();
responseStatus.response = ResponseType.NONE;
responseStatus.time = OffsetDateTimeSerializer.deserialize("datetime-value");
event.responseStatus = responseStatus;
event.recurrence = null;
event.iCalUId = "iCalUId-value";
event.reminderMinutesBeforeStart = 99;
event.isOnlineMeeting = true;
event.onlineMeetingProvider = OnlineMeetingProviderType.TEAMS_FOR_BUSINESS;
event.isReminderOn = true;
event.hideAttendees = false;
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Red category");
event.categories = categoriesList;

graphClient.me().events("{id}")
    .buildRequest()
    .patch(event);

```