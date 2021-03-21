---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04045d80b552e2dd017fbfc35f9ff78866df2ddc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = new PlannerBucketTaskBoardTaskFormat();
plannerBucketTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("{task-id}").bucketTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerBucketTaskBoardTaskFormat);

```