---
title: tipo de recurso fileAttachment
description: 'Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um evento, mensagem ou postagem. O  **contentBytes** '
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ba313838a7481e436019abd224397a9f138be591072c4b369a1ad572e72ed857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218727"
---
# <a name="fileattachment-resource-type"></a>tipo de recurso fileAttachment

Namespace: microsoft.graph

Um arquivo (como um arquivo de texto ou um documento do Word) anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md) do usuário. 

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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

