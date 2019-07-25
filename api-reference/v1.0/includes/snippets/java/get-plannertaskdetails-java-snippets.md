---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fad35cd5433feb9eaedc2aff39a6772103447bad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888760"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskDetails plannerTaskDetails = graphClient.planner().tasks("{task-id}").details()
    .buildRequest()
    .get();

```