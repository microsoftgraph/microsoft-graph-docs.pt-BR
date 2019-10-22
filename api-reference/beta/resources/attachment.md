---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 0ab32470a7ecf5e00d10ccada984096d16537f1b
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632665"
---
# <a name="attachment-resource-type"></a>tipo de recurso anexo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode adicionar conteúdo relacionado a um [evento](../resources/event.md)de usuário, [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) de grupo no formato de um anexo. 

Os eventos em calendários de grupo não têm suporte para anexos.

**attachment** é o recurso de base para os seguintes tipos de anexo derivados:

* Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))
* Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))
* Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))

>**Observação**: há um limite para o tamanho do arquivo ou anexo de item que pode ser adicionado abaixo de 4 MB. 
>
> No entanto, se estiver anexando a uma mensagem um arquivo entre 3 MB e 150MB, você pode [criar uma sessão de carregamento](../api/attachment-createuploadsession.md) e carregar de forma iterativa os intervalos do arquivo para anexá-lo. Consulte [anexar arquivos grandes às mensagens do Outlook](/graph/outlook-large-attachments) para obter um exemplo.

## <a name="methods"></a>Métodos

Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter anexo](../api/attachment-get.md) | [anexo](attachment.md) |Leia as propriedades, relações ou conteúdo bruto de um anexo, anexados a um evento de usuário, mensagem, tarefa do Outlook ou postagem.|
|[Adicionar anexo a um evento do usuário](../api/event-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.|
|[Adicionar um anexo a uma mensagem](../api/message-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma mensagem. Esta operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.|
|[Criar sessão para anexar arquivo grande](../api/attachment-createuploadsession.md)| [uploadSession](uploadsession.md) | Criar uma sessão de carregamento que permite que um aplicativo carregue intervalos de um arquivo de forma iterativa, para anexar o arquivo à **mensagem**especificada. O tamanho do arquivo deve estar entre 3 MB e 150MB.|
|[Adicionar anexo a uma tarefa do Outlook](../api/outlooktask-post-attachments.md) | [attachment](attachment.md) |Adicionar um anexo de arquivo, item ou link a uma tarefa do Outlook.|
|[Adicionar anexo a uma postagem](../api/post-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma postagem.|
|[Listar anexos de um evento de usuário](../api/event-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de um evento em um calendário de usuário. |
|[Listar anexos de uma mensagem](../api/message-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma mensagem. |
|[Listar anexos de uma tarefa do Outlook](../api/outlooktask-list-attachments.md) | Coleção [attachment](attachment.md) | Obter uma lista de anexos para uma tarefa do Outlook. |
|[Listar anexos de uma postagem](../api/post-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma postagem. |
|[Delete](../api/attachment-delete.md) | None |Excluir um anexo de um evento, de uma mensagem, de uma tarefa do Outlook ou de uma postagem. |

## <a name="properties"></a>Propriedades

A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo MIME.|
|id|String| Somente leitura.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|nome|Cadeia de caracteres|O nome de exibição do anexo. Não precisa ser o nome real do arquivo.|
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
  "suppressions": []
}
-->
