---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ccdc8259d7ce109e80b02fe169a4184e36fa1286
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137479"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments("AAMkADKoAAA=")
    .cancel(BookingAppointmentCancelParameterSet
        .newBuilder()
        .withCancellationMessage(cancellationMessage)
        .build())
    .buildRequest()
    .post();

```