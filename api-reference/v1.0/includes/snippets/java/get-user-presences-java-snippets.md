---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 030ac9e6a209b27af15bbf5ca16af8e47fda112d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Presence presence = graphClient.communications().presences("dc74d9bb-6afe-433d-8eaa-e39d80d3a647")
    .buildRequest()
    .get();

```