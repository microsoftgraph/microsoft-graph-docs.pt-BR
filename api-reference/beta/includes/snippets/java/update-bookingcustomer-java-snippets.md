---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 982afa073c489ac082b9d1802a348b636d5a96702aa78a62cac9f2494cc6f386
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899105"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = new BookingCustomer();
bookingCustomer.displayName = "Adele";
bookingCustomer.emailAddress = "adele@relecloud.com";

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers("8bb19078-0f45-4efb-b2c5-da78b860f73a")
    .buildRequest()
    .patch(bookingCustomer);

```