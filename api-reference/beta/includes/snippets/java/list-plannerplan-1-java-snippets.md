---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70177da1f7d0ceb856cb4f801e23ae65fc583d597aab211406a9ab33b3d19f18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271921"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionWithReferencesPage plans = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").plans()
    .buildRequest()
    .get();

```