---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf9d6928da88cdc9640bbb8941c3588a545de0f6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871015"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "clientContext-value";

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .unmute(clientContext)
    .buildRequest()
    .post();

```