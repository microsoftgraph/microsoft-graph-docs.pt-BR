---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acbd3c83f89dc699f67581289a6f66db77cfcbcb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965937"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10002")
    .buildRequest()
    .delete();

```