---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563071"
---
# <a name="referenceattachment-resource-type"></a>Tipo de recurso referenceAttachment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) .

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
|id|Cadeia de caracteres|A ID do anexo.  Somente leitura.|
|isFolder|Booliano|Especifica se o anexo é um link para uma pasta. Deve definir this como true se **sourceUrl** for um link para uma pasta. Opcional.|
|isInline|Booliano|Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação. Opcional.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional.|
|name|String|O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo. Obrigatório.|
|autorização|ReferenceAttachmentPermissions|Especifica as permissões concedidas para o anexo pelo tipo de provedor no **ProviderType**. Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Opcional.|
|previewUrl|String|Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem de visualização. Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|
|providerType|ReferenceAttachmentProviders|O tipo de provedor que dá suporte a um anexo deste contentType. Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Opcional.|
|size|Int32|O tamanho dos metadados em bytes armazenados na mensagem para o anexo de referência. Esse valor não indica o tamanho real do arquivo. Opcional.|
|Urlorigem|String|URL para obter o conteúdo do anexo. Se esta for uma URL para uma pasta, para que a pasta seja exibida corretamente no Outlook ou no Outlook na Web, defina **IsFolder** como true. Obrigatório.|
|thumbnailUrl|String|Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem em miniatura. Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|

## <a name="relationships"></a>Relações
Nenhum



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
