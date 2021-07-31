---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c675d79598ff4428f3384518edc74cfcb8cc050d
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665855"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>Tipo de recurso appliedConditionalAccessPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|conditionsSatisfied|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que são atendidas. Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|conditionsNotSatisfied|conditionalAccessConditions|Refere-se às condições de política de acesso condicional que não estão atendidas. Os valores possíveis são: `none`, `application`, `users`, `devicePlatform`, `location`, `clientType`, `signInRisk`, `userRisk`, `time`, `deviceState`, `client`.|
|enforcedGrantControls|Coleção de cadeias de caracteres|Refere-se aos controles de concessão imposto pela política de acesso condicional (exemplo: "Exigir autenticação multifacional").|
|enforcedSessionControls|Coleção de cadeias de caracteres|Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados ao aplicativo").|
|id|Cadeia de caracteres|Identificador da política de acesso condicional.|
|resultado|appliedConditionalAccessPolicyResult| Indica o resultado da política de AC que foi disparada. Os valores possíveis são: , , , (A política não é aplicada porque as condições de política não foram atendidas), (Isso ocorre devido à política em estado `success` desabilitado), , , , , `failure` , `notApplied` `notEnabled` `unknown` `unknownFutureValue` `reportOnlySuccess` `reportOnlyFailure` `reportOnlyNotApplied` . `reportOnlyInterrupted` Observe que você deve usar o header de solicitação para obter os seguintes valores nesta `Prefer: include-unknown-enum-members` [enum evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `reportOnlySuccess` , , , `reportOnlyFailure` `reportOnlyNotApplied` `reportOnlyInterrupted` .|

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
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
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
