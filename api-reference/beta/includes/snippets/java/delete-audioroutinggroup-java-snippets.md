---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c35d2f33ebf99b632d8eb170a26b91720e0b1297
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961607"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .delete();

```