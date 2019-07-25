---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0987540388dd16c6023038084184ca527a806639
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859270"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = "true";

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```