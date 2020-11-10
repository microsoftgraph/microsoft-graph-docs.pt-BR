---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e943203e4f46b7ed3a91c99bbad001cfbf9a644e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978224"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = graphClient.planner().plans("{id}")
    .buildRequest()
    .get();

```