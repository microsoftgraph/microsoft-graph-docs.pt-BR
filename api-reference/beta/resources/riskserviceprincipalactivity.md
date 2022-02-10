---
title: Tipo de recurso riskServicePrincipalActivity
description: Representa a atividade de risco de uma entidade de serviço do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD.
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d73f77adbc44833a489270b64e51006eaab49896
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519946"
---
# <a name="riskserviceprincipalactivity-resource-type"></a>Tipo de recurso riskServicePrincipalActivity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Representa a atividade de risco de uma entidade de serviço do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD. 

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|riskEventType|String|O tipo de evento de risco detectado. Os valores possíveis são: `unlikelyTravel`, `anonymizedIPAddress`, , `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, , `suspiciousIPAddress``leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, , `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, , `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
| detail     | riskDetail  | Detalhes do risco detectado. <br>**Observação:** detalhes para esta propriedade estão disponíveis apenas para clientes do Azure AD Premium P2. Clientes P1 serão retornados `hidden`. <br/>Os valores possíveis são: `none`, `adminGeneratedTemporaryPassword`, , `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, , `userPassedMFADrivenByRiskBasedPolicy``aiConfirmedSigninSafe`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, , `adminConfirmedUserCompromised`, `unknownFutureValue`, , `adminConfirmedServicePrincipalCompromised`, `adminDismissedAllRiskForServicePrincipal`. Observe que você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter os seguintes valores nesta [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `adminConfirmedServicePrincipalCompromised` , `adminDismissedAllRiskForServicePrincipal`.|

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskServicePrincipalActivity"
}-->
```json
{
    "riskEventTypes": ["String"],
    "detail": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->

