---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbb1df5ed26b9373a8453d5df918a8e379d54fda71cbdee1a845beeebb4ef439
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157650"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = new BookingAppointment();
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2018-05-06T12:30:00+00:00";
end.timeZone = "UTC";
bookingAppointment.end = end;
DateTimeTimeZone invoiceDate = new DateTimeTimeZone();
invoiceDate.dateTime = "2018-05-06T12:30:00+00:00";
invoiceDate.timeZone = "UTC";
bookingAppointment.invoiceDate = invoiceDate;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2018-05-06T12:00:00+00:00";
start.timeZone = "UTC";
bookingAppointment.start = start;

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .patch(bookingAppointment);

```