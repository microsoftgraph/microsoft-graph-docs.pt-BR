---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1edb3a12c3c8eb9e3177311dc82c591425c24589
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864612"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .unmute(clientContext)
    .buildRequest()
    .post();

```