---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4642f3369fb48a9e31233bbfa7ac3bd19e2a751ac605f4626e2ca4e0384d1e62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailboxSettings mailboxSettings = new MailboxSettings();
WorkingHours workingHours = new WorkingHours();
workingHours.endTime = new TimeOfDay(0, 0, 0);
LinkedList<DayOfWeek> daysOfWeekList = new LinkedList<DayOfWeek>();
daysOfWeekList.add(DayOfWeek.MONDAY);
daysOfWeekList.add(DayOfWeek.TUESDAY);
daysOfWeekList.add(DayOfWeek.WEDNESDAY);
daysOfWeekList.add(DayOfWeek.THURSDAY);
daysOfWeekList.add(DayOfWeek.FRIDAY);
daysOfWeekList.add(DayOfWeek.SATURDAY);
workingHours.daysOfWeek = daysOfWeekList;
CustomTimeZone timeZone = new CustomTimeZone();
timeZone.bias = -300;
timeZone.name = "Customized Time Zone";
StandardTimeZoneOffset standardOffset = new StandardTimeZoneOffset();
standardOffset.time = new TimeOfDay(0, 0, 0);
standardOffset.dayOccurrence = 2;
standardOffset.dayOfWeek = DayOfWeek.SUNDAY;
standardOffset.month = 10;
standardOffset.year = 0;
timeZone.standardOffset = standardOffset;
DaylightTimeZoneOffset daylightOffset = new DaylightTimeZoneOffset();
daylightOffset.daylightBias = 100;
daylightOffset.time = new TimeOfDay(0, 0, 0);
daylightOffset.dayOccurrence = 4;
daylightOffset.dayOfWeek = DayOfWeek.SUNDAY;
daylightOffset.month = 5;
daylightOffset.year = 0;
timeZone.daylightOffset = daylightOffset;
workingHours.timeZone = timeZone;
mailboxSettings.workingHours = workingHours;

graphClient.customRequest("/me/mailboxSettings", MailboxSettings.class)
    .buildRequest()
    .patch(mailboxSettings);

```