---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8262f464cd68a6f17be1f44f865138d8b1fe8de9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888774"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTask plannerTask = graphClient.planner().tasks("{task-id}")
    .buildRequest()
    .get();

```