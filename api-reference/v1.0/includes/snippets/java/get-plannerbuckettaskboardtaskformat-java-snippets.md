---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 600d8d86209e6a3d179cf1b62467914a17fc7259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970140"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = graphClient.planner().tasks("{task-id}").bucketTaskBoardFormat()
    .buildRequest()
    .get();

```