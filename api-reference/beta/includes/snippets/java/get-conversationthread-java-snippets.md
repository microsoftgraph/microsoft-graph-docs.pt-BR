---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 699f4df88c11e5241084787335c3772e0d38f71a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862922"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThread conversationThread = graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .get();

```