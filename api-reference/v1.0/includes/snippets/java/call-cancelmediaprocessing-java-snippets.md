---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c40e8916eb51c97ece854872b193adbec5759ec1
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330098"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}")
    .cancelMediaProcessing(clientContext)
    .buildRequest()
    .post();

```