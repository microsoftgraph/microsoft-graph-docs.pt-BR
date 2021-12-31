---
title: Tipo de recurso authenticationRequirementPolicy
description: O Azure AD pode exigir que os usuários passem uma verificação MFA antes de acessar recursos. Se uma verificação MFA for necessária, esse recurso identificará a política que requer MFA.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 287a946321e72bb2ff5002c0ed21ad0d1267b313
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647196"
---
# <a name="authenticationrequirementpolicy-resource-type"></a>Tipo de recurso authenticationRequirementPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Azure AD pode exigir que os usuários passem uma verificação MFA antes de acessar recursos. Se uma verificação MFA for necessária, esse recurso identificará a política que requer MFA. 


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|detail|String|Fornece detalhes adicionais sobre o recurso identificado em requirementProvider.|
|requirementProvider|requirementProvider|Identifica qual recurso do Azure AD requer MFA nesta política. Os valores possíveis são: `user`, `request`, `servicePrincipal`, `v1ConditionalAccess`, `multiConditionalAccess`, `tenantSessionRiskPolicy`, `accountCompromisePolicies`, `v1ConditionalAccessDependency`, `v1ConditionalAccessPolicyIdRequested`, `mfaRegistrationRequiredByIdentityProtectionPolicy`, `baselineProtection`, `mfaRegistrationRequiredByBaselineProtection`, `mfaRegistrationRequiredByMultiConditionalAccess`, `enforcedForCspAdmins`, `securityDefaults`, `mfaRegistrationRequiredBySecurityDefaults`, `proofUpCodeRequest`, `crossTenantOutboundRule`, `gpsLocationCondition`, `riskBasedPolicy`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationRequirementPolicy",
  "requirementProvider": "String",
  "detail": "String"
}
```
