---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3038ea51552b3aad15399509e7d5b0313e29c5f3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953207"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlow identityUserFlow = new IdentityUserFlow();
identityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
identityUserFlow.userFlowTypeVersion = 1;

graphClient.identity().userFlows()
    .buildRequest()
    .post(identityUserFlow);

```