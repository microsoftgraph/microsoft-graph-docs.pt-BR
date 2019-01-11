---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para a unidade de nuvem de negócios ou outros locais de armazenamento suportadas, anexado ao '
localization_priority: Normal
ms.openlocfilehash: 6a334b303bea7aff768733434b9ba882de237a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880049"
---
# <a name="referenceattachment-resource-type"></a>Tipo de recurso referenceAttachment

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um link para uma pasta ou um arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para Business cloud unidade ou outro suporte para locais de armazenamento anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md) .

Derivado de [attachment](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get](../api/attachment-get.md) | [referenceAttachment](referenceattachment.md) |Leia as propriedades e os relacionamentos do objeto referenceAttachment.|
|[Delete](../api/attachment-delete.md) | Nenhum |Exclua o objeto referenceAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|Cadeia de caracteres|O tipo de conteúdo do anexo. Opcional.|
|id|Cadeia de caracteres|A ID do anexo.  Somente leitura.|
|isFolder|Booliano|Especifica se o anexo é um link para uma pasta. Defina essa opção para true se **sourceUrl** é um link para uma pasta. Opcional.|
|isInline|Booliano|Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação. Opcional.|
|lastModifiedDateTime|DateTimeOffset|Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional.|
|name|Cadeia de caracteres|O texto que é exibido abaixo do ícone que representa o anexo incorporado. Isso não precisa ser o nome de arquivo real. Obrigatório.|
|permissão|ReferenceAttachmentPermissions|Especifica as permissões concedidas pelo tipo de provedor na **providerType**o anexo. Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`. Opcional.|
|previewUrl|Cadeia de caracteres|Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem de visualização. Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|
|providerType|ReferenceAttachmentProviders|O tipo de provedor que ofereça suporte a um anexo deste contentType. Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`. Opcional.|
|size|Int32|O tamanho dos metadados em bytes que é armazenado na mensagem do anexo da referência. Esse valor não indica o tamanho real do arquivo. Opcional.|
|Urlorigem|Cadeia de caracteres|URL para obter o conteúdo do anexo. Se essa for uma URL para uma pasta, em seguida, para a pasta para serem exibidos corretamente no Outlook ou no Outlook na web, defina **isFolder** como true. Obrigatório.|
|thumbnailUrl|Cadeia de caracteres|Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem em miniatura. Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem. Opcional.|

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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
