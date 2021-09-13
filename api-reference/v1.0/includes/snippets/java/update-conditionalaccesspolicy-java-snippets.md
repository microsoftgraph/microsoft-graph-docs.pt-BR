---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4062ccfde570088aba56cd316e8c54d4764e4c55b8846b89e262adf7efa4c124
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326919"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
LinkedList<RiskLevel> signInRiskLevelsList = new LinkedList<RiskLevel>();
signInRiskLevelsList.add(RiskLevel.HIGH);
signInRiskLevelsList.add(RiskLevel.MEDIUM);
signInRiskLevelsList.add(RiskLevel.LOW);
conditions.signInRiskLevels = signInRiskLevelsList;
conditionalAccessPolicy.conditions = conditions;

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .patch(conditionalAccessPolicy);

```