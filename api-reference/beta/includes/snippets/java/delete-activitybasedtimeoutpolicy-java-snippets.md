---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 828543489cbf8365ca0e3651d7b2ebcb31ca4418
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .delete();

```