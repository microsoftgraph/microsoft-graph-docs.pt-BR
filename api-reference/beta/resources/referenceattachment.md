---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e0c3723648710fb1640927fad10e0847e1e155a6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721317"
---
# <a name="referenceattachment-resource-type"></a>Tipo de recurso referenceAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a um evento [,](../resources/event.md)mensagem [ou](../resources/message.md) [postagem](../resources/post.md) .

Derivado de [attachment](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |Leia as propriedades e os relacionamentos do objeto referenceAttachment.|
|[Delete](../api/attachment-delete.md) | Nenhum(a) |Exclua o objeto referenceAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo de conteúdo do anexo. Opcional.|
|id|Cadeia de caracteres|A ID do anexo.  Somente leitura.|
|isFolder|Booliano|Especifica se o anexo é um link para uma pasta. Deve definir isso como true se **sourceUrl** for um link para uma pasta. Opcional.|
|isInline|Booliano|Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação. Opcional.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional.|
|nome|Cadeia de caracteres|O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo. Obrigatório.|
|permission|referenceAttachmentPermission|Especifica as permissões concedidas para o anexo pelo tipo de provedor em **providerType**. Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Opcional.|
|previewUrl|Cadeia de caracteres|Aplica-se apenas a um anexo de referência de uma imagem - URL para obter uma imagem de visualização. Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identificar um arquivo de imagem. Opcional.|
|providerType|referenceAttachmentProvider|O tipo de provedor que dá suporte a um anexo desse contentType. Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Opcional.|
|size|Int32|O tamanho dos metadados em bytes armazenados na mensagem para o anexo de referência. Esse valor não indica o tamanho real do arquivo. Opcional.|
|Urlorigem|Cadeia de caracteres|URL para obter o conteúdo do anexo. Se essa for uma URL para uma pasta, para que a pasta seja exibida corretamente no Outlook ou no Outlook na Web, de definir **isFolder** como true. Obrigatório.|
|thumbnailUrl|Cadeia de caracteres|Aplica-se apenas a um anexo de referência de uma imagem - URL para obter uma imagem em miniatura. Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identificar um arquivo de imagem. Opcional.|

## <a name="relationships"></a>Relações
Nenhum



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


