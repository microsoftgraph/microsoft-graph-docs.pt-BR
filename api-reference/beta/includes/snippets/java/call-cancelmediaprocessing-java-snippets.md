---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c40e8916eb51c97ece854872b193adbec5759ec1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959819"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}")
    .cancelMediaProcessing(clientContext)
    .buildRequest()
    .post();

```