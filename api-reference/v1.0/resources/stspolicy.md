---
title: Tipo de recurso stsPolicy
description: Representa um tipo de base abstrato para tipos de política que controlam o comportamento da plataforma de identidade da Microsoft.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ba7afc9d338a0fd34b5548ca2ade69eebfecf29c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760887"
---
# <a name="stspolicy-resource-type"></a>Tipo de recurso stsPolicy

Namespace: microsoft.graph

Representa um tipo de base abstrato para tipos de política que controlam o [comportamento da plataforma de identidade da Microsoft.](/azure/active-directory/develop/)

Herda de [policyBase](policyBase.md).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador exclusivo dessa política. Somente leitura. Herdado de [policyBase](policyBase.md).|
|descrição|String| Descrição dessa política. Herdado de [policyBase](policyBase.md).|
|displayName|String| Nome de exibição para esta política. Herdado de [policyBase](policyBase.md).|
|definition|Coleção de cadeias de caracteres| Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações de uma política. A sintaxe da definição difere para cada tipo de política derivado. Obrigatório.|
|isOrganizationDefault|Booliano|Se definido como true, ativa essa política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização. Opcional, o valor padrão é false.|

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