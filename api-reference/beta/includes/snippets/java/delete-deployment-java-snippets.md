---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e805c60928b68b2245d263dab0f2dab9d6163424
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241373"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().deployments("{deploymentId}")
    .buildRequest()
    .delete();

```