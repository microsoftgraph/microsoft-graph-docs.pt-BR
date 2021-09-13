---
title: Tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 140402be929fc6d0d906b084251e21bab80f1a24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59078963"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>Tipo de recurso appliedConditionalAccessPolicy

Namespace: microsoft.graph

Indica os atributos relacionados à política de acesso condicional ou políticas aplicadas que são disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Refere-se ao Nome da política de acesso condicional (exemplo: "Exigir MFA para Salesforce").|
|enforcedGrantControls|Coleção String|Refere-se aos controles de concessão imposto pela política de acesso condicional (exemplo: "Exigir autenticação multifacional").|
|enforcedSessionControls|Coleção String|Refere-se aos controles de sessão impostos pela política de acesso condicional (exemplo: "Exigir controles aplicados ao aplicativo").|
|id|Cadeia de caracteres|Um identificador da política de acesso condicional.|
|resultado|appliedConditionalAccessPolicyResult| Indica o resultado da política de AC que foi disparada. Os valores possíveis são: , , , (A política não é aplicada porque as condições de política não foram atendidas), (Isso ocorre devido à política em estado `success` `failure` `notApplied` `notEnabled` desabilitado), `unknown` , `unknownFutureValue` .|

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

