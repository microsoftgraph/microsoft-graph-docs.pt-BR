---
title: tipo de recurso de conditionalAccessPolicy
description: Indica que os atributos relacionados a uma política de acesso condicional ou diretivas que é disparado pela atividade correspondente entrar
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820640"
---
# <a name="conditionalaccesspolicy-resource-type"></a>tipo de recurso de conditionalAccessPolicy
Indica que os atributos relacionados a uma política de acesso condicional ou diretivas que é disparado pela atividade correspondente entrar



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|Refere-se com o nome da política de acesso condicional (exemplo: "Exigir MFA para a equipe de vendas").|
|enforcedGrantControls|String collection|Refere-se aos controles grant impostos com a política de acesso condicional (exemplo: "Exigem a autenticação multifator").|
|enforcedSessionControls|String collection|Refere-se aos controles sessão impostos com a política de acesso condicional (exemplo: "Exigem controles app imposto").|
|id|Cadeia de caracteres|GUID exclusivo da política de acesso condicional|
|result|Cadeia de caracteres| Indica o resultado da política de autoridade de certificação que tiver sido disparado. Valores possíveis são:<br/> `success` <br/> `failure` <br/> `notApplied`-Diretiva não será aplicada, porque as condições da diretiva não foram atendidas. <br/> `notEnabled`-Isso acontece devido à política em estado desabilitado.|

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
