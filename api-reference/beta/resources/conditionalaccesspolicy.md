---
title: tipo de recurso conditionalAccessPolicy
description: Indica os atributos relacionados a uma política de acesso condicional ou políticas disparadas pela atividade de entrada correspondente
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2c45be8ee32c26187ccf42154ba6c06b60f5efc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973213"
---
# <a name="conditionalaccesspolicy-resource-type"></a>tipo de recurso conditionalAccessPolicy
Indica os atributos relacionados a uma política de acesso condicional ou políticas disparadas pela atividade de entrada correspondente



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|Refere-se ao nome da política de acesso condicional (exemplo: "exigir MFA de Salesforce").|
|enforcedGrantControls|Coleção de cadeias de caracteres|Refere-se aos controles Grant impostos pela política de acesso condicional (exemplo: "requer autenticação multifator").|
|enforcedSessionControls|Coleção de cadeias de caracteres|Refere-se aos controles de sessão aplicados pela política de acesso condicional (exemplo: "exigir controles de aplicação imposta)").|
|id|String|GUID exclusivo da política de acesso condicional|
|resultado|String| Indica o resultado da política de autoridade de certificação que foi disparada. Os valores possíveis são:<br/> `success` <br/> `failure` <br/> `notApplied`-A política não é aplicada porque as condições da política não foram atendidas. <br/> `notEnabled`– Isso ocorre devido à política em estado desabilitado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
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
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
