---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4562481e20a25d1c79c825cdc4ff63b46f0f7885
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776281"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().patents("{id}")
    .buildRequest()
    .delete();

```