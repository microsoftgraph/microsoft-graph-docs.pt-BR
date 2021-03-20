---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8394b846a80246ed804e53879a97798889d814fa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966693"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCustomer bookingCustomer = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").customers("8bb19078-0f45-4efb-b2c5-da78b860f73a")
    .buildRequest()
    .get();

```