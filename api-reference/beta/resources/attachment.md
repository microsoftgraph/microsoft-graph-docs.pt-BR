---
title: tipo de recurso attachment
description: Você pode adicionar conteúdo relacionado a um evento,
localization_priority: Normal
ms.openlocfilehash: 59e1074cea9508af45cef0b6e61ea223a3ca851e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526939"
---
# <a name="attachment-resource-type"></a>tipo de recurso attachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md) na forma de um anexo.

**attachment** é o recurso de base para os seguintes tipos de anexo derivados:

* Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))
* Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))
* Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))

## <a name="methods"></a>Métodos

Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter anexo](../api/attachment-get.md) | [attachment](attachment.md) |Leia as propriedades e relacionamentos de um anexo, anexados a um evento, mensagem, tarefa do Outlook ou postagem.|
|[Adicionar anexo a um event](../api/event-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a um evento.|
|[Adicionar um anexo a uma mensagem](../api/message-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma mensagem.|
|[Adicionar anexos para uma tarefa do Outlook](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma tarefa do Outlook.|
|[Adicionar anexo a uma postagem](../api/post-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma postagem.|
|[Listar anexos de um evento](../api/event-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de um evento. |
|[Listar anexos de uma mensagem](../api/message-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma mensagem. |
|[Listar anexos de uma tarefa do Outlook](../api/outlooktask-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos para uma tarefa do Outlook. |
|[Listar anexos de uma postagem](../api/post-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma postagem. |
|[Delete](../api/attachment-delete.md) | Nenhum |Exclua um anexo em um evento, mensagem, tarefa do Outlook ou postagem. |

## <a name="properties"></a>Propriedades

A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo MIME.|
|id|String| Somente leitura.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Isso não precisa ser o nome de arquivo real.|
|size|Int32|O comprimento do anexo em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
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
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
