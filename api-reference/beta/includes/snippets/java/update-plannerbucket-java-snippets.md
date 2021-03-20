---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61555a50b171813050f4186c595c535385e64c18
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Development";

graphClient.planner().buckets("hsOf2dhOJkqyYYZEtdzDe2QAIUCR")
    .buildRequest( requestOptions )
    .patch(plannerBucket);

```