---
title: Tipo de recurso itemAttachment
description: 'Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.  '
ms.localizationpriority: high
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: 92c9b42c70780d564e252dbde5cef39734c6afd3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084311"
---
# <a name="itemattachment-resource-type"></a>Tipo de recurso itemAttachment

Namespace: microsoft.graph

Um contato, evento ou mensagem anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md) do usuário.  

Derivado de [attachment](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |Leia as propriedades, os relacionamentos ou o conteúdo bruto de um objeto itemAttachment.|
|[Delete](../api/attachment-delete.md) | Nenhum |Exclua o objeto itemAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo de conteúdo do anexo.|
|id|String| A ID do anexo.|
|isInline|Booliano|Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.|
|lastModifiedDateTime|DateTimeOffset|Última data e hora em que o anexo foi alterado.|
|name|Cadeia de caracteres|O nome de exibição do anexo.|
|size|Int32|O tamanho do anexo em bytes.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|A mensagem ou evento anexado. Propriedade de navegação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

