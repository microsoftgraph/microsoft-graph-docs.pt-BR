---
title: tipo de recurso appliedConditionalAccessPolicy
description: Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c90e8b012e62317b1a8b02df723d9426ec99c282
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003357"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a>tipo de recurso appliedConditionalAccessPolicy

Namespace: microsoft.graph

Indica os atributos relacionados à política ou políticas de acesso condicional aplicadas que são disparadas pela atividade de entrada correspondente.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").|
|enforcedGrantControls|Coleção de cadeias de caracteres|Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").|
|enforcedSessionControls|Coleção de cadeias de caracteres|Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").|
|id|String|GUID exclusivo da política de acesso condicional.|
|resultado|String| Indica o resultado da política de autoridade de certificação que foi disparada. Os valores possíveis são:<br/>`success`<br/>`failure`<br/>`notApplied` -A política não é aplicada porque as condições da política não foram atendidas.<br/>`notEnabled` – Isso ocorre devido à política em estado desabilitado.|

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

