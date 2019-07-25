---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffb5569f2ad847b9b6e09fb38e58a57c5b944d2f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857280"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKqAAA=")
    .buildRequest()
    .delete();

```