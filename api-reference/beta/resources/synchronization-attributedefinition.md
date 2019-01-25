---
title: tipo de recurso de attributeDefinition
description: Descreve um atributo de um objeto.
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514338"
---
# <a name="attributedefinition-resource-type"></a>tipo de recurso de attributeDefinition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve um atributo de um objeto.

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição    |
|:--------------|:----------|:---------------|
|Âncora         |Booliano    | `true`Se o atributo deve ser usado como a âncora do objeto. Atributos de âncora devem ter um valor exclusivo que identifica um objeto e devem ser imutáveis. O padrão é `false`. Um e somente um dos atributos do objeto devem ser designado como a âncora para oferecer suporte à sincronização. |
|caseExact      |Booliano    |`true`Se o valor desse atributo deve ser tratado como diferencia maiusculas de minúsculas. Essa configuração afeta como o mecanismo de sincronização detecta alterações para o atributo.|
|Metadata       |[metadataEntry](../resources/synchronization-metadataentry.md)    |Propriedades adicionais de extensão. A menos que mencionado explicitamente, valores de metadados não devem ser alterados.|
|Valores múltiplos    |Booliano    |`true`Se um atributo pode ter vários valores. O padrão é `false`.|
|Mutabilidade     |String     |Mutabilidade de um atributo. Os valores possíveis são: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`. O padrão é `ReadWrite`.|
|name           |Cadeia de caracteres     |Nome do atributo. Deve ser exclusivo dentro da definição do objeto. Não anulável.|
|obrigatório       |Booliano    |`true`Se o atributo é necessário. Objeto não pode ser criado se qualquer um dos atributos necessários estão ausentes. Se durante a sincronização, o atributo required não tiver nenhum valor, o valor padrão será usado. Se o valor do padrão não foi definido, a sincronização irá registrar um erro.|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) |Para atributos com `reference` digitar, listas de objetos referenciados (por exemplo, o `manager` atributo seria listar `User` como o objeto referenciado).|
|type           |String     |Tipo de valor do atributo. Os valores possíveis são: `String`, `Integer`, `Reference`, `Binary`, `Boolean`. O padrão é `String`.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
