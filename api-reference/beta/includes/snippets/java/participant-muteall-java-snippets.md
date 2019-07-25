---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35f6b035ce18e1b20e1b7001d189c7fcaa58d0c4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877020"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> participantsList = new LinkedList<String>();
participantsList.add("");

String clientContext = "clientContext-value";

graphClient.app().calls("{id}").participants()
    .muteAll(participantsList,clientContext)
    .buildRequest()
    .post();

```