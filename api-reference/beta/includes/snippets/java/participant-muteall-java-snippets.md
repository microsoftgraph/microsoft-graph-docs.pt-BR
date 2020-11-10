---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63be0762778e588b3ea37072622f45b8c39d9595
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968726"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> participantsList = new LinkedList<String>();
participantsList.add("");

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}").participants()
    .muteAll(participantsList,clientContext)
    .buildRequest()
    .post();

```