---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de3d109c8f6fb0cf116a0faeed412d818401d3d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974686"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingCurrency bookingCurrency = graphClient.bookingCurrencies("USD")
    .buildRequest()
    .get();

```