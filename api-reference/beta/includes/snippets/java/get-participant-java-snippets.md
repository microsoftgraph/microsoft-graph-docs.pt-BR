---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f46d266a1ec2c48f1098d139a3f4326e903a9dc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Participant participant = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants("7e1b4346-85a6-4bdd-abe3-d11c5d420efe")
    .buildRequest()
    .get();

```