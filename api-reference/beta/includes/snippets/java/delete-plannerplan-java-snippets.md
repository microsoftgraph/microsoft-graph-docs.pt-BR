---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 132009e93988b7e2734178515c4b5e79f3b4d170
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

graphClient.planner().plans("'id'")
    .buildRequest( requestOptions )
    .delete();

```