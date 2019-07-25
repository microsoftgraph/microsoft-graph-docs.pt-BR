---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 897ad4112b70bdfb461198da8e2f52e1f7f48983
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865482"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com")
    .publish(bookingBusiness)
    .buildRequest()
    .post();

```