---
title: Tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de signin.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bc5123975dc15c7c49f0dcbec507c345cf057850
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761048"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a>Tipo de recurso signInFrequencySessionControl

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Controle de sessão para impor a frequência de login. Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isEnabled     |Booliano      | Especifica se o controle de sessão está habilitado. |
|tipo          |Cadeia de caracteres       | Os valores possíveis são: `days` e `hours`.|
|valor         |Int32        | O número de `days` ou `hours` .|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


