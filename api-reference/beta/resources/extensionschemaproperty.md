---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: extensions
author: keylimesoda
ms.openlocfilehash: 346237a22914dffb3dde708d7d272de44bf37b0d
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556007"
---
# <a name="extensionschemaproperty-resource-type"></a>Tipo de recurso extensionSchemaProperty

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|nome|Cadeia de caracteres| O nome da propriedade fortemente tipada definida como parte de uma extensão de esquema.|
|type|Cadeia de caracteres| O tipo da propriedade que é definida como parte de uma extensão de esquema.  Os valores permitidos `Binary`são `Boolean`, `DateTime`, `Integer` ou `String`. Consulte a tabela abaixo para obter mais detalhes.|

### <a name="supported-property-data-types"></a>Tipos de dados de propriedade com suporte 
Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:

| Tipo de propriedade | Comentários |
|-------------|------------|
| Binária | No máximo 256 bytes. |
| Booliano | Não é compatível com as mensagens, eventos e postagens. |
| DateTime | Deve ser especificado no formato ISO 8601. Serão armazenados no UTC. |
| Inteiro | Valor de 32 bits. Não é compatível com as mensagens, eventos e postagens. |
| String | Máximo de 256 caracteres. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


