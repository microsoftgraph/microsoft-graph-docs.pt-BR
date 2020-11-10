---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411d997ea542d53bf56e4674b5d0cb0df78f011a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981615"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().messages("{id}")
    .copy(destinationId)
    .buildRequest()
    .post();

```