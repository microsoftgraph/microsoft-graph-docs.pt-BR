---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7459c6bacfcb5b34e0df820151b86039b73645c9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865720"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RejectReason reason = RejectReason.NONE;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .reject(reason,null)
    .buildRequest()
    .post();

```