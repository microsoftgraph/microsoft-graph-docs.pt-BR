---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e84e0bd736cde78f4e001fb0a0717edcfe60f33cfcbaf451c550a2bacb5bf7b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = graphClient.planner().buckets("{bucket-id}")
    .buildRequest()
    .get();

```