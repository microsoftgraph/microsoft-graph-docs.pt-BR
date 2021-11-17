---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36ce0c6e94677756f539dd10dad7c6a22d20583969c7f8a3af134e134f020a3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157653"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKoAAA=")
    .cancel(BookingAppointmentCancelParameterSet
        .newBuilder()
        .withCancellationMessage(cancellationMessage)
        .build())
    .buildRequest()
    .post();

```