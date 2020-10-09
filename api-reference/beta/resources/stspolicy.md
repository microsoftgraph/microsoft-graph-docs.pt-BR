---
title: tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 078284cb4134b0b4fa2f86eb9a09f61ab6655351
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405278"
---
# <a name="stspolicy-resource-type"></a>tipo de recurso stsPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de base abstrato para tipos de política que controlam o comportamento da [plataforma de identidade da Microsoft](/azure/active-directory/develop/) .

Herda de [policyBase](policyBase.md).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo da política. Somente leitura. Herdado de [policyBase](policyBase.md).|
|description|Cadeia de caracteres| Descrição da política. Herdado de [policyBase](policyBase.md).|
|displayName|Cadeia de caracteres| Nome para exibição dessa política. Herdado de [policyBase](policyBase.md).|
|definir|Conjunto de cadeias de caracteres| Uma coleção String contendo uma cadeia de caracteres JSON que define as regras e configurações de uma política. A sintaxe da definição difere para cada tipo de política derivada. Obrigatório.|
|isOrganizationDefault|Boolean|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->