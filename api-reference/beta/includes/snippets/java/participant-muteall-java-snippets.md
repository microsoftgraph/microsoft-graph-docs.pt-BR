---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9471aeb9fe7c59729b7c5aa1157f8c1369c228f5f105d844c0b4f15b36f433a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160323"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> participantsList = new LinkedList<String>();
participantsList.add("");

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}").participants()
    .muteAll(ParticipantMuteAllParameterSet
        .newBuilder()
        .withParticipants(participantsList)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```