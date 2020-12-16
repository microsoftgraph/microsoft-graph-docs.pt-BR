---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc96406fd2e3dae22d7bd83fbdc3e453f07d6eb3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690027"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").tabs("d731fca0-0f14-4537-971a-0ef9101ff13d")
    .buildRequest()
    .delete();

```