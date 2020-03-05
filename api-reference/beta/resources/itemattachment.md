---
title: Tipo de recurso itemAttachment
description: Um contato, evento ou mensagem que está anexado a outro evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 82f0e9fa1ab499d7adc305cd74fcf7cdf09fd796
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523090"
---
# <a name="itemattachment-resource-type"></a>Tipo de recurso itemAttachment

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contato, evento ou mensagem anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.  

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
|item|[OutlookItem](outlookitem.md)|O contato anexado, a mensagem ou o evento. Propriedade de navegação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
