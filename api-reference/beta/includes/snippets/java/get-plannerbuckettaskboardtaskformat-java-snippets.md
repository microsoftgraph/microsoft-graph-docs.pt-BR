---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7af6a875087902ffdd30c8cb452c4c7f846c2a5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876508"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketTaskBoardTaskFormat plannerBucketTaskBoardTaskFormat = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh").bucketTaskBoardFormat()
    .buildRequest()
    .get();

```