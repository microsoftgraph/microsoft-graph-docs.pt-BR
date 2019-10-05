---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5cc2fb7d41ccaba17d76ae012d6dd9fdc83f63e
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402667"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(groupId,renameAs,null,null,null)
    .buildRequest()
    .post();

```