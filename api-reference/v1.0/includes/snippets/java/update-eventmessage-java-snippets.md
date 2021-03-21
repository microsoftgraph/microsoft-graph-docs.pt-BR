---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67e50f6599ca88804a9346394be14a2cdd355414
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973295"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = true;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```