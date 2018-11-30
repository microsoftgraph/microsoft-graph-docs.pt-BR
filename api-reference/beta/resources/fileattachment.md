---
title: tipo de recurso fileAttachment
description: Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um evento,
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037337"
---
# <a name="fileattachment-resource-type"></a>tipo de recurso fileAttachment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um arquivo (por exemplo, um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md). A propriedade **contentBytes** contém o conteúdo do arquivo codificado na base64.  

Ao criar um anexo de arquivo, inclua o seguinte no corpo da solicitação:

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* As propriedades **name** e **contentBytes** necessárias.

Derivado de [attachment](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [fileAttachment](fileattachment.md) |Leia as propriedades e os relacionamentos do objeto fileAttachment.|
|[Delete](../api/attachment-delete.md) | Nenhuma |Exclua um objeto fileAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentBytes|Binária|O conteúdo do arquivo codificado pela base64.|
|contentId|String|A ID do anexo no repositório do Exchange.|
|contentLocation|String|O URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.|
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
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
