---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3bad8cbfef7dbf3f44c804e33ff5ab62726a4d8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876480"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = new PlannerBucketTaskBoardTaskFormat();
plannerBucketTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("hsOf2dhOJkqyYYZEtdzDe2QAIUCR").bucketTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerBucketTaskBoardTaskFormat);

```