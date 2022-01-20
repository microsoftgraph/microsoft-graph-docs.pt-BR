---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a016775a094ded28304febc3ab83819704e621a2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114095"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("start", "2018-04-30T00:00:00Z"));
requestOptions.add(new QueryOption("end", "2018-05-10T00:00:00Z"));

BookingAppointmentCollectionPage calendarView = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").calendarView()
    .buildRequest( requestOptions )
    .get();

```