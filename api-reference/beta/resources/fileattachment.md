---
title: tipo de recurso fileAttachment
description: Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1ef32e91897ac322b84922012df47c168094f57d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135643"
---
# <a name="fileattachment-resource-type"></a>tipo de recurso fileAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Um arquivo (como um arquivo de texto ou documento do Word) anexado a um evento de usuário [,](../resources/event.md) [mensagem](../resources/message.md), tarefa do [Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md). 

Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* As propriedades **name** e **contentBytes** necessárias.

Derivado de [attachment](attachment.md).

> [!NOTE]
> Certifique-se de codificar o conteúdo do arquivo em Base64 antes de atribuí-lo a **contentBytes**.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Leia as propriedades, relações ou conteúdo bruto de um objeto fileAttachment.|
|[Delete](../api/attachment-delete.md) | Nenhuma |Exclua um objeto fileAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentBytes|Edm.Binary|O conteúdo do arquivo codificado pela base64.|
|contentId|String|A ID do anexo no repositório do Exchange.|
|contentLocation|Cadeia de caracteres|Não use essa propriedade que não tem suporte.|
|contentType|String|O tipo de conteúdo do anexo.|
|id|String|A ID do anexo.|
|isInline|Booliano|Defina como true se este for um anexo embutido.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez.|
|name|String|O nome que representa o texto que é exibido abaixo do ícone que representa o anexo inserido. Não precisa ser o nome de arquivo real.|
|size|Int32|O tamanho do anexo em bytes.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


