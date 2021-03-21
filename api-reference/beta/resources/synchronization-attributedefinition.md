---
title: Tipo de recurso attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956810"
---
# <a name="attributedefinition-resource-type"></a>Tipo de recurso attributeDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um atributo de um objeto.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|anchor         |Booliano    | `true` se o atributo deve ser usado como âncora para o objeto. Os atributos de âncora devem ter um valor exclusivo que identifique um objeto e devem ser imutáveis. O padrão é `false`. Um e apenas um dos atributos do objeto devem ser designados como âncora para dar suporte à sincronização. |
|caseExact      |Booliano    |`true` se o valor desse atributo deve ser tratado como sensível a caso. Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.|
|flowNullValues |Booliano    |'true' para permitir valores nulos para atributos.|
|metadados       |[Coleção metadataEntry](../resources/synchronization-metadataentry.md)   |Propriedades de extensão adicionais. A menos que mencionado explicitamente, os valores de metadados não devem ser alterados.|
|multivalued    |Booliano    |`true` se um atributo pode ter vários valores. O padrão é `false`.|
|mutabilidade     |mutabilidade     |Mutabilidade de um atributo. Os valores possíveis são:  `ReadWrite` `ReadOnly` , , , `Immutable` `WriteOnly` . O padrão é `ReadWrite`.|
|nome           |Cadeia de caracteres     |Nome do atributo. Deve ser exclusivo na definição do objeto. Não anulável.|
|obrigatório       |Booliano    |`true` se o atributo for necessário. O objeto não poderá ser criado se nenhum dos atributos necessários estiver ausente. Se durante a sincronização, o atributo necessário não tiver valor, o valor padrão será usado. Se o valor padrão não foi definido, a sincronização registrará um erro.|
|referencedObjects|[Coleção referencedObject](../resources/synchronization-referencedobject.md) |Para atributos com `reference` tipo, lista objetos referenciados (por exemplo, o `manager` atributo listaria `User` como o objeto referenciado).|
|tipo           |attributeType     |Tipo de valor de atributo. Os valores possíveis `String` são: `Integer` , , , , , `Reference` `Binary` `Boolean` `DateTime` . O padrão é `String`.|

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


