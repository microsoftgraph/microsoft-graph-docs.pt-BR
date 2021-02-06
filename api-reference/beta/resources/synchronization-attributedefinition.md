---
title: Tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128810"
---
# <a name="attributedefinition-resource-type"></a>Tipo de recurso attributeDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um atributo de um objeto.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|âncora         |Boolean    | `true` se o atributo deve ser usado como âncora para o objeto. Os atributos de âncora devem ter um valor exclusivo que identifique um objeto e devem ser imutáveis. O padrão é `false`. Um e apenas um dos atributos do objeto devem ser designados como a âncora para suportar a sincronização. |
|caseExact      |Boolean    |`true` se o valor desse atributo deve ser tratado como sensível a minúsculas. Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.|
|flowNullValues |Boolean    |"true" para permitir valores nulos para atributos.|
|metadados       |[Coleção metadataEntry](../resources/synchronization-metadataentry.md)   |Propriedades de extensão adicionais. A menos que seja mencionado explicitamente, os valores de metadados não devem ser alterados.|
|multivalorado    |Boolean    |`true` se um atributo puder ter vários valores. O padrão é `false`.|
|mutability     |String     |A transformabilidade de um atributo. Os valores possíveis `ReadWrite` são: `ReadOnly` , , `Immutable` . `WriteOnly` O padrão é `ReadWrite`.|
|nome           |String     |Nome do atributo. Deve ser exclusivo na definição do objeto. Não anulável.|
|obrigatório       |Boolean    |`true` se o atributo for necessário. O objeto não poderá ser criado se nenhum dos atributos necessários estiver faltando. Se, durante a sincronização, o atributo necessário não tiver valor, o valor padrão será usado. Se o valor padrão não foi definido, a sincronização registrará um erro.|
|referencedObjects|[Coleção referencedObject](../resources/synchronization-referencedobject.md) |Para atributos com `reference` tipo, listas de objetos referenciados (por exemplo, o `manager` atributo listaria `User` como o objeto referenciado).|
|type           |String     |Tipo de valor de atributo. Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. O padrão é `String`.|

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
  "flowNullValues": true,
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


