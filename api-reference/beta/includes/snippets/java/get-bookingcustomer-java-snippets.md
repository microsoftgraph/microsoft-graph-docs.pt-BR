---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6acbdd20707d692da23d0640d6b521a5ed95fcba
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113950"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").customers("8bb19078-0f45-4efb-b2c5-da78b860f73a")
    .buildRequest()
    .get();

```