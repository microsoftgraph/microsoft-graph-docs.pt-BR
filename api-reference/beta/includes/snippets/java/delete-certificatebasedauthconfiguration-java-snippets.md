---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 657d8834f700d06a98aaea8004a0bfd85c481552
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959441"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("{id}").certificateBasedAuthConfiguration("{id}")
    .buildRequest()
    .delete();

```