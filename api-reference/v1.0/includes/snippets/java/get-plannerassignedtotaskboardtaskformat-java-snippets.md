---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf05f5605b502c421f8b07c528d2d59ce41c77ef
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892175"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").assignedToTaskBoardFormat()
    .buildRequest()
    .get();

```