---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c12e1cc0b2cff9ed3e8976fe82f09b552607644c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968298"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}").jobs("{id}")
    .cancel()
    .buildRequest()
    .post();

```