---
title: tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb5562b07e60b10a36dafac37d5839d9bacc060a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629338"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>tipo de recurso appliedConditionalAccessPolicy

Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").|
|enforcedGrantControls|Coleção de cadeias de caracteres|Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").|
|enforcedSessionControls|Coleção de cadeias de caracteres|Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").|
|id|Cadeia de caracteres|GUID exclusivo da vigilância de acesso condicional. y|
|resultado|Cadeia de caracteres| Indica o resultado da política de autoridade de certificação que foi disparada. Os valores possíveis são:<br/>`success`<br/>`failure`<br/>`notApplied`-A política não é aplicada porque as condições da política não foram atendidas.<br/>`notEnabled`– Isso ocorre devido à política em estado desabilitado.|

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
