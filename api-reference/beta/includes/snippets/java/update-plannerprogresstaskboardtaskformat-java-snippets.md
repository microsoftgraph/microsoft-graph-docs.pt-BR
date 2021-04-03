---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b18c5ad427359168a9898b18c956511b36a25bff
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573058"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = new PlannerProgressTaskBoardTaskFormat();
plannerProgressTaskBoardTaskFormat.orderHint = "A6673H Ejkl!";

graphClient.planner().tasks("{id}").progressTaskBoardFormat()
    .buildRequest( requestOptions )
    .patch(plannerProgressTaskBoardTaskFormat);

```