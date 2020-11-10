---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81cbde01204a2323b9a6ff34d642473694d16fe1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972408"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = graphClient.termStore().sets("{setId}")
    .buildRequest()
    .get();

```