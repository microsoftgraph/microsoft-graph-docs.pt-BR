---
title: tipo de recurso anexo
description: Você pode adicionar conteúdo relacionado a um evento
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 3faea96a9ef9c19c2d5471c1cc6f58ed84b9a2ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721625"
---
# <a name="attachment-resource-type"></a>tipo de recurso anexo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Você pode adicionar conteúdo relacionado a um evento [de](../resources/event.md)usuário, [mensagem,](../resources/message.md)tarefa do [Outlook](../resources/outlooktask.md)ou postagem de grupo na forma de um anexo. [](../resources/post.md) 

Os eventos em calendários de grupo não têm suporte para anexos.

As tarefas do Outlook não suportam anexos de referência.

**attachment** é o recurso de base para os seguintes tipos de anexo derivados:

* Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))
* Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))
* Um link para um arquivo (recurso [referenceAttachment](../resources/referenceattachment.md))

>**Observação**: há um limite para o tamanho do anexo de arquivo ou item que você pode adicionar a menos de 4 MB. 
>
> No entanto, se você estiver anexando a uma mensagem um arquivo que esteja entre 3MB e 150 MB, você pode criar uma sessão de [carregamento](../api/attachment-createuploadsession.md) e carregar iterativamente intervalos do arquivo para anexá-lo. Consulte [anexar arquivos grandes a mensagens do Outlook](/graph/outlook-large-attachments) para um exemplo.

## <a name="methods"></a>Métodos

Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter anexo](../api/attachment-get.md) | [attachment](attachment.md) |Leia as propriedades, relações ou conteúdo bruto de um anexo, anexado a um evento de usuário, mensagem, tarefa do Outlook ou postagem.|
|[Adicionar anexo a um evento do usuário](../api/event-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a um evento em um calendário de usuário.|
|[Adicionar um anexo a uma mensagem](../api/message-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma mensagem. Essa operação limita o tamanho do anexo que você pode adicionar a menos de 4 MB.|
|[Criar sessão para anexar um arquivo grande](../api/attachment-createuploadsession.md)| [uploadSession](uploadsession.md) | Crie uma sessão de carregamento que permita que um aplicativo carregue iterativamente intervalos de um arquivo, para anexar o arquivo à mensagem **especificada**. O tamanho do arquivo deve estar entre 3MB e 150 MB.|
|[Adicionar anexo a uma tarefa do Outlook](../api/outlooktask-post-attachments.md) (preterida) | [attachment](attachment.md) |Adicione um arquivo ou anexo de item a uma tarefa do Outlook.|
|[Adicionar anexo a uma postagem](../api/post-post-attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma postagem de grupo.|
|[Listar anexos de um evento de usuário](../api/event-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de um evento em um calendário de usuário. |
|[Listar anexos de uma mensagem](../api/message-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma mensagem. |
|[Listar anexos de uma tarefa](../api/outlooktask-list-attachments.md) do Outlook (preterida) | Coleção [attachment](attachment.md) | Obter uma lista de anexos para uma tarefa do Outlook. |
|[Listar anexos de uma postagem](../api/post-list-attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma postagem. |
|[Delete](../api/attachment-delete.md) | Nenhum(a) |Exclua um anexo em um evento, mensagem, tarefa do Outlook ou postagem. |

## <a name="properties"></a>Propriedades

A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceattachment.md)) para propriedades adicionais.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo MIME.|
|id|String| Somente leitura.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
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


