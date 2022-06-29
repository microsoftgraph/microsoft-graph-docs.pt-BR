---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb1acacc255441b5ab52538565e063cd33924ce3
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.chats("19:cf66807577b149cca1b7af0c32eec122@thread.v2").pinnedMessages("1616964509832")
    .buildRequest()
    .delete();

```