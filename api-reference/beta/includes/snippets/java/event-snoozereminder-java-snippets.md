---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8088a23497561edbf3941087fc79b56b5ef3da31
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954743"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DateTimeTimeZone newReminderTime = new DateTimeTimeZone();
newReminderTime.dateTime = "2016-10-19T10:37:00Z";
newReminderTime.timeZone = "timeZone-value";

graphClient.me().events("{id}")
    .snoozeReminder(newReminderTime)
    .buildRequest()
    .post();

```