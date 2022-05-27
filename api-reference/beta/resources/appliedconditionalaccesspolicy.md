---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional aplicada ou às políticas disparadas pela atividade de entrada correspondente.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fe1f31555c2ea809d50faf87a1041f527a5ddc74
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695332"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>Tipo de recurso appliedConditionalAccessPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica os atributos relacionados à política de acesso condicional aplicada ou às políticas disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|authenticationStrength|[authenticationStrength](authenticationstrength.md)| A força de autenticação personalizada imposta em uma política de Acesso Condicional.|
|conditionsNotSatisfied|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que não são atendidas. Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, , `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, , `client`,`ipAddressSeenByAzureAD`,,`ipAddressSeenByResourceProvider`,`unknownFutureValue`,.`servicePrincipals``servicePrincipalRisk` Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals`,`servicePrincipalRisk`.|
|conditionsSatisfied|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que são atendidas. Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, , `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, , `client`,`ipAddressSeenByAzureAD`,,`ipAddressSeenByResourceProvider`,`unknownFutureValue`,.`servicePrincipals``servicePrincipalRisk` Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `servicePrincipals`,`servicePrincipalRisk`.|
|displayName|String|Nome da política de acesso condicional.|
|enforcedGrantControls|Coleção de cadeias de caracteres|Refere-se aos controles de concessão impostos pela política de acesso condicional (exemplo: "Exigir autenticação multifator").|
|enforcedSessionControls|Coleção de cadeias de caracteres|Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados pelo aplicativo").|
|excludeRulesSatisfied|[Coleção conditionalAccessRuleSatisfied](conditionalaccessrulesatisfied.md)|Lista de pares chave-valor que contêm cada condição de exclusão correspondente na política de acesso condicional. Exemplo: `[{"devicePlatform" : "DevicePlatform"}]` significa que a política não se aplicava, porque a condição DevicePlatform era uma correspondência.|
|id|Cadeia de caracteres|Identificador da política de acesso condicional.|
|includeRulesSatisfied|[Coleção conditionalAccessRuleSatisfied](conditionalaccessrulesatisfied.md)|Lista de pares chave-valor que contêm cada condição de inclusão correspondente na política de acesso condicional. Exemplo: `[{ "application" : "AllApps"}, {"users": "Group"}]`, o que significa que a condição de aplicativo foi uma correspondência porque  AllApps estão incluídos e a condição Usuários era uma correspondência porque o usuário fazia parte da regra de grupo incluída.|
|resultado|appliedConditionalAccessPolicyResult| Indica o resultado da política de AC que foi disparada. Os valores possíveis são: , , (A política não é aplicada porque as condições de política não foram atendidas),`notEnabled` (Isso ocorre devido à política no estado desabilitado), `unknown`, `unknownFutureValue`, `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`. `notApplied` `failure``success` Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores nesta [enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `reportOnlySuccess`, `reportOnlyFailure`, `reportOnlyNotApplied`, `reportOnlyInterrupted`.|
|sessionControlsNotSatisfied|Coleção de cadeias de caracteres|Refere-se aos controles de sessão que uma atividade de entrada não satisfaça. (Exemplo: `Application enforced Restrictions`).|




## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
}-->

```json
{
  "@odata.type": "#microsoft.graph.appliedConditionalAccessPolicy",
  "id": "String (identifier)",
  "authenticationStrength": {"@odata.type": "microsoft.graph.authenticationStrength"},
  "displayName": "String",
  "enforcedGrantControls": [
    "String"
  ],
  "enforcedSessionControls": [
    "String"
  ],
  "conditionsSatisfied": "String",
  "conditionsNotSatisfied": "String",
  "includeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "excludeRulesSatisfied": [
    {
      "@odata.type": "microsoft.graph.conditionalAccessRuleSatisfied"
    }
  ],
  "result": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
