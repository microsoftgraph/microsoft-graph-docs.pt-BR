---
title: Tipo de recurso extensionSchemaProperty
description: Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição schemaExtension.
localization_priority: Normal
ms.openlocfilehash: 384f60c323ca6c6fb23d2f4811a6d2cb918bf844
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575783"
---
# <a name="extensionschemaproperty-resource-type"></a>Tipo de recurso extensionSchemaProperty

Use o recurso **extensionSchemaProperty** para definir o nome da propriedade e o tipo dela, como parte de uma definição [schemaExtension](schemaextension.md).


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|String| O nome da propriedade fortemente tipada definido como parte de uma extensão de esquema.|
|type|String| O tipo da propriedade digitada definido como parte de uma extensão de esquema.  Os valores permitidos são: *Binary, Boolean, DateTime, Integer* ou *String*.  Confira a tabela abaixo para ver mais detalhes.|

#### <a name="supported-property-data-types"></a>Tipos de dados de propriedade com suporte 
Há suporte para os seguintes tipos de dados quando se define uma propriedade em uma extensão do esquema:

| Tipo de propriedade | Comentários |
|-------------|------------|
| Binária | No máximo 256 bytes. |
| Booliano | Não é compatível com os contatos, mensagens, eventos e postagens. |
| DateTime | Deve ser especificado no formato ISO 8601. Serão armazenados no UTC. |
| Inteiro | Valor de 32 bits. Não é compatível com os contatos, mensagens, eventos e postagens. |
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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
