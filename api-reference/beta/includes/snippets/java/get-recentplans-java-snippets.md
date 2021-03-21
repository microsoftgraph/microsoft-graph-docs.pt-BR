---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b85eb58157c3b9cb4d433abc4ff3d10d2f4310d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage recentPlans = graphClient.me().planner().recentPlans()
    .buildRequest()
    .get();

```