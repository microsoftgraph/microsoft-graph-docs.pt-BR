---
title: tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac3f6e18c4775f45f6a36814ea09b16914e139d3
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218447"
---
# <a name="attributedefinition-resource-type"></a>tipo de recurso attributeDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um atributo de um objeto.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|Core         |Boolean    | `true`Se o atributo deve ser usado como a âncora do objeto. Atributos de âncora devem ter um valor exclusivo que identifica um objeto e deve ser imutável. O padrão é `false`. Um, e apenas um, dos atributos do objeto deve ser designado como a âncora para dar suporte à sincronização. |
|caseExact      |Boolean    |`true`Se o valor desse atributo deve ser tratado como diferencia maiúsculas de minúsculas. Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.|
|los       |coleção [metadataEntry](../resources/synchronization-metadataentry.md)   |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|
|múltiplos valores    |Boolean    |`true`se um atributo puder ter vários valores. O padrão é `false`.|
|Imutabilidade     |Cadeia de Caracteres     |Uma imutabilidade de atributo. Os valores possíveis são `ReadWrite`: `ReadOnly`, `Immutable`, `WriteOnly`,. O padrão é `ReadWrite`.|
|nome           |String     |Nome do atributo. Deve ser exclusivo dentro da definição do objeto. Não anulável.|
|obrigatório       |Boolean    |`true`Se o atributo for necessário. Objeto não pode ser criado se qualquer um dos atributos necessários estiver ausente. Se durante a sincronização, o atributo Required não tem valor, o valor padrão será usado. Se o valor padrão não foi definido, a sincronização registrará um erro.|
|referencedObjects|coleção [referenciable](../resources/synchronization-referencedobject.md) |Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, `manager` o atributo seria `User` List como o objeto referenciado).|
|tipo           |String     |Tipo de valor de atributo. Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. O padrão é `String`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
