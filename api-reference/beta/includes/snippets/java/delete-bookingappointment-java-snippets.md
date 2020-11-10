---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffb5569f2ad847b9b6e09fb38e58a57c5b944d2f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960967"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKqAAA=")
    .buildRequest()
    .delete();

```