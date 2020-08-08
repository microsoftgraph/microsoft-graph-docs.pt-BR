---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8aed4c0370c18051c27719629848b49da93daac
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566052"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
LinkedList<String> signInRiskLevelsList = new LinkedList<String>();
signInRiskLevelsList.add("high");
signInRiskLevelsList.add("medium");
signInRiskLevelsList.add("low");
conditions.signInRiskLevels = signInRiskLevelsList;
conditionalAccessPolicy.conditions = conditions;

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .patch(conditionalAccessPolicy);

```