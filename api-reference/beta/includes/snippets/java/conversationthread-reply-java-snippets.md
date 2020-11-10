---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e59869ee0f864e23b31432480167551711856027
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
post.body = body;

graphClient.groups("{id}").threads("{id}")
    .reply(post)
    .buildRequest()
    .post();

```