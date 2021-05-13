---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7320de7fc81d1955d5adaa74fd916bf0ec48b606
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRule unifiedRoleManagementPolicyRule = new UnifiedRoleManagementPolicyRule();
UnifiedRoleManagementPolicyRuleTarget target = new UnifiedRoleManagementPolicyRuleTarget();
unifiedRoleManagementPolicyRule.target = target;

graphClient.policies().roleManagementPolicies("{unifiedRoleManagementPolicyId}").rules("{unifiedRoleManagementPolicyRuleId}")
    .buildRequest()
    .patch(unifiedRoleManagementPolicyRule);

```