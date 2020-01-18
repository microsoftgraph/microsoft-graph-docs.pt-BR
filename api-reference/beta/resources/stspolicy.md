---
title: tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f351d994daba00f4465d934fe570b5db2e704ae9
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234058"
---
# <a name="policybase-resource-type"></a>tipo de recurso policyBase

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de base abstrato para tipos de política que controlam o comportamento da [plataforma de identidade da Microsoft](https://docs.microsoft.com/azure/active-directory/develop/) .

Herda de [policyBase](policyBase.md).

## <a name="methods"></a>Métodos

Nenhuma

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo da política. Somente leitura. Herdado de [policyBase](policyBase.md).|
|description|String| Descrição da política. Herdado de [policyBase](policyBase.md).|
|displayName|Cadeia de caracteres| Nome para exibição dessa política. Herdado de [policyBase](policyBase.md).|
|definir|Coleção de cadeias de caracteres| Uma coleção String contendo uma cadeia de caracteres JSON que define as regras e configurações de uma política. A sintaxe da definição difere para cada tipo de política derivada. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|

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