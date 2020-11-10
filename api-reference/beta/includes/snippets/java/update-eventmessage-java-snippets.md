---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3c2e95f5ac82c2f29a52de4518743b8ab62b81d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965703"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = false;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```