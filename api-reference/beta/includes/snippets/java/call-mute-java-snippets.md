---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4d759010438b2cf4746f06b9f2d180ceeabcb33
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959644"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .mute(clientContext)
    .buildRequest()
    .post();

```