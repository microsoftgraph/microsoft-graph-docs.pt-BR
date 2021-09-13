---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f387a65b3936bd57c400a8d26b1d2afc983a6ac8d4cc222ef3484b67bd8d4b6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159468"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.groups("{group-id}").planner().plans()
    .buildRequest()
    .get();

```