---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c595bf454215bf6b46c325494bcc8f0f813ef118
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

graphClient.me().messages("{id}")
    .replyAll(null,comment)
    .buildRequest()
    .post();

```