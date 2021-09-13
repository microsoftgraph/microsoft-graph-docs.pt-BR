---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24493efcf964f7fef46447f141334b0a8d00c4b6fe376efae734ba67d90265e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099299"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.planner().plans()
    .buildRequest()
    .get();

```