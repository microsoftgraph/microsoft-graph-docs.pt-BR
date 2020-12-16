---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a644783525ac9e5961fd0fe43c8526d7f061f4a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689150"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> idsList = new LinkedList<String>();
idsList.add("fa8bf3dc-eca7-46b7-bad1-db199b62afc3");
idsList.add("66825e03-7ef5-42da-9069-724602c31f6b");

graphClient.communications()
    .getPresencesByUserId(idsList)
    .buildRequest()
    .post();

```