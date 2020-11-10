---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc2cc89c5cc46199659ca346f18428e604b67d89
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954960"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Cancelling for this week due to all hands";

graphClient.me().events("{id}")
    .cancel(comment)
    .buildRequest()
    .post();

```