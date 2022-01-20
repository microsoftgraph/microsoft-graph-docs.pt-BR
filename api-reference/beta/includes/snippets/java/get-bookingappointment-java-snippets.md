---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c17862d5e1ed9f113556f6842496110341a88ee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .get();

```