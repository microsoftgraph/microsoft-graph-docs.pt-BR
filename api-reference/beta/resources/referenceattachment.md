---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 426d746305b2a8418fb30515720d888226d3da74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462209"
---
# <a name="referenceattachment-resource-type"></a>Tipo de recurso referenceAttachment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md)ou [postagem](../resources/post.md) .

Derivado de [attachment](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |Leia as propriedades e os relacionamentos do objeto referenceAttachment.|
|[Excluir](../api/attachment-delete.md) | None |Exclua o objeto referenceAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo de conteúdo do anexo. Opcional.|
|id|String|A ID do anexo.  Somente leitura.|
|isFolder|Booliano|Especifica se o anexo é um link para uma pasta. Deve definir this como true se **sourceUrl** for um link para uma pasta. Opcional.|
|isInline|Booliano|Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação. Opcional.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional.|
|nome|Cadeia de caracteres|O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo. Obrigatório.|
|autorização|referenceAttachmentPermission|Especifica as permissões concedidas para o anexo pelo tipo de provedor no **ProviderType**. Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Opcional.|
|previewUrl|String|Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem de visualização. Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|
|providerType|referenceAttachmentProvider|O tipo de provedor que dá suporte a um anexo deste contentType. Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Opcional.|
|size|Int32|O tamanho dos metadados em bytes armazenados na mensagem para o anexo de referência. Esse valor não indica o tamanho real do arquivo. Opcional.|
|Urlorigem|String|URL para obter o conteúdo do anexo. Se esta for uma URL para uma pasta, para que a pasta seja exibida corretamente no Outlook ou no Outlook na Web, defina **IsFolder** como true. Obrigatório.|
|thumbnailUrl|String|Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem em miniatura. Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|

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
